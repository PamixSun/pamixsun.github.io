---
layout: post
title:  "ROC Analysis Tool based on DeLong's Method"
date:   2015-8-31
categories: update
---

# Background

CLASSIFICATION is an important framework of data analysis that extracts models describing and distinguishing data classes and concepts associated with the observed dataset.
To evalute the performance of a classification algorithm, accuracy is widely employed as an empirical validation index in practice.
However, as criticized by some researchers, accuracy can sometimes be misleading, and should be replaced or complemented with the metric associated with receiver operating characteristic (ROC) analysis.

Originated from problems of radar and sonar detection in early 1950s, receiver operating characteristic (ROC) analysis has become an indispensable tool to tackle
the so-called two-sample problems in many scientific and engineering fields, such as describing the performances of diagnostic systems in clinical medicine, characterizing the
overall accuracies of classifiers in machine learning, quantifying the extent of signal detectability in signal processing, and so forth.

In essence, ROC analysis is a supervised research framework that requires prior knowledge of both the sample membership and underlying cumulative distribution functions (cdfs)
generating the two samples.
Given such knowledge, the procedure of ROC analysis might be initiated from plotting a two-dimensional ROC curve, which is traced out by pairs of false-positive rate and true-positive rate according to various decision threshold settings.
With the ROC curve, the area under the curve (AUC) can then be computed, either analytically or empirically, as a figure of merit that might be better than accuracy when characterizing a classifier’s performance.

As revealed by Bamber, AUC can be estimated by the Mann-Whitney U statistic (MWUS).
Based on such relationship, a plenty of nonparametric methods have been proposed in the literature.
Among algorithms for comparing the areas under two or more correlated receiver operating characteristic (ROC) curves, DeLong’s algorithm is perhaps the most widely used
one due to its simplicity of implementation in practice.
Recently, we have reduced the time complexity of DeLong’s algorithm from quadratic down to linearithmic order, based on an equivalent relationship between the Heaviside function and mid-ranks of samples.

In this post, I will release the sourse codes of the two algorithms that mentioned in our paper, and then give a brief introduction of a ROC analysis tool that published in my github page.

**Soure codes**

Since our method is based on the relationship between Heaviside function and mid-ranks of samples, the first step is to calculate the mid-ranks. Below is the MATLAB code to acheive that. The input of this function, namely, $x$, is a one by $N$ vector, and the output is the corresponding mid-ranks.

*Algorithm 1: Procedure of Calculating Mid-ranks*

    function T = midrank(x)
    %MIDRANK
    [Z J] = sort(x);
    Z = [Z Z(end) + 1];
    N = length(x);
    T = zeros(1, N);
    i = 1;
    while i <= N
        a = i;
        j = a;
        while Z(j) == Z(a)
            j = j + 1;
        end
            b = j - 1;
        for k = a : b
            T(k) = (a + b) / 2;
        end
        i = b + 1;
    end
    T(J) = T;
    end

With the *midrank* function, now we are ready to implement the fast version of DeLong's algorithm, which is showed below as algorithm 2. In this function, the input argument, namely, $samples$, is a struct in MATLAB consisted with two elements:
- $spsizes$ is a $2 * 1$ vector, which represent the sizes of two samples, namely, $X$ and $Y$, and can be denoted by $m$ and $n$, respectively.
- $ratings$ is a $K * N$ matrix, where each row represents the ratings of one experiments. Note that $N$ must be equal to the sum of $m$ and $n$, and its first $m$ elements is the ratings corresponding to $X$, while the last $n$ corresonding to $Y$.

*Algorithm 2: Improved DeLong’s Algorithm*

    function [aucs, delongcov] = fastDeLong(samples)
    %FASTDELONGCOV
    %The fast version of DeLong's method for computing the covariance of 
    %unadjusted AUC.
    %% [aucs, delongcov] = fastDeLong(samples)
    %% 
    
    if sum(samples.spsizes) ~= size(samples.ratings, 2) || numel(samples.spsizes) ~= 2
        error('Argument mismatch error');
    end
    
    z = samples.ratings;
    m = samples.spsizes(1);
    n = samples.spsizes(2);
    x = z(:, 1 : m);
    y = z(:, m + 1 : end);
    k = size(z, 1);
    
    tx = zeros(k, m);
    ty = zeros(k, n);
    tz = zeros(k, m + n);
    
    for r = 1 : k
        tx(r, :) = midrank(x(r, :));
        ty(r, :) = midrank(y(r, :));
        tz(r, :) = midrank(z(r, :));
    end
    
    aucs = sum(tz(:, 1 : m), 2) / m / n - (m + 1) / 2 / n;
    
    v01 = (tz(:, 1 : m) - tx(:, :)) / n;
    v10 = 1 - (tz(:, m + 1 : end) - ty(:, :)) / m;
    
    sx = cov(v01')';
    sy = cov(v10')';
    
    delongcov = sx / m + sy / n;
    
    end


****Introduction of the ROC analysis tool****

Furthur more, I have published a UI tool for ROC analysis in my github page, you can download the sourse code here.



![plot of chunk unnamed-chunk-4](/images/delong/image_1.png)
 
![plot of chunk unnamed-chunk-4](/images/delong/image_2.png) 


**Citation Request**

If you publish material based on these codes, then, please refer to our paper:

    X. Sun, W. Xu, Fast implementation of DeLong's algorithm for comparing the areas under correlated receiver operating characteristic curves, IEEE Signal Processing Letters 21 (11) (2014) 1389{1393.

Here is a BiBTeX citation as well:

    @article{sun2014fast,
      title={Fast Implementation of DeLong's Algorithm for Comparing the Areas Under Correlated Receiver Operating Characteristic Curves},
      author={Xu Sun and Weichao Xu},
      journal={IEEE Signal Processing Letters},
      volume={21},
      number={11},
      pages={1389--1393},
      year={2014},
      publisher={IEEE}
    }


