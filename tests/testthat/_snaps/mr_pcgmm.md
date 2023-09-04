# pcgmm applied to standard object

    Code
      mr_pcgmm(Input1, nx = 17723, ny = 17723)
    Output
      
      Univariable principal components generalized method of moments (PC-GMM) method
      
      Number of principal components used : 13 
      
      Robust model with overdispersion heterogeneity.
      
      ------------------------------------------------------------------
       Method Estimate Std Error 95% CI       p-value F-stat
       PC-GMM    3.241     0.774 1.724, 4.757   0.000   47.3
      ------------------------------------------------------------------
      
      Overdispersion heterogeneity parameter estimate = 81.75673 
      
      Heterogeneity test statistic = 11.9284

# pcgmm with r changed

    Code
      mr_pcgmm(Input1, nx = 17723, ny = 17723, r = 4)
    Output
      
      Univariable principal components generalized method of moments (PC-GMM) method
      
      Number of principal components used : 4 
      
      Robust model with overdispersion heterogeneity.
      
      ------------------------------------------------------------------
       Method Estimate Std Error 95% CI       p-value F-stat
       PC-GMM    2.490     0.460 1.590, 3.391   0.000   75.4
      ------------------------------------------------------------------
      
      Overdispersion heterogeneity parameter estimate = -6.916574 
      
      Heterogeneity test statistic = 0.7974

# pcgmm with thres changed

    Code
      mr_pcgmm(Input1, nx = 17723, ny = 17723, thres = 0.85)
    Output
      
      Univariable principal components generalized method of moments (PC-GMM) method
      
      Number of principal components used : 3 
      
      Robust model with overdispersion heterogeneity.
      
      ------------------------------------------------------------------
       Method Estimate Std Error 95% CI       p-value F-stat
       PC-GMM    2.469     0.471 1.546, 3.393   0.000   95.1
      ------------------------------------------------------------------
      
      Overdispersion heterogeneity parameter estimate = -6.247456 
      
      Heterogeneity test statistic = 0.7572

# pcgmm with robust off

    Code
      mr_pcgmm(Input1, nx = 17723, ny = 17723, robust = FALSE)
    Output
      
      Univariable principal components generalized method of moments (PC-GMM) method
      
      Number of principal components used : 13 
      
      Non-robust model with no overdispersion heterogeneity.
      
      ------------------------------------------------------------------
       Method Estimate Std Error 95% CI       p-value F-stat
       PC-GMM    3.033     0.336 2.375, 3.692   0.000   47.3
      ------------------------------------------------------------------
      
      Heterogeneity test statistic = 46.6439 on 12 degrees of freedom, (p-value = 0.0000)

# pcgmm with alpha changed

    Code
      mr_pcgmm(Input1, nx = 17723, ny = 17723, alpha = 0.001)
    Output
      
      Univariable principal components generalized method of moments (PC-GMM) method
      
      Number of principal components used : 13 
      
      Robust model with overdispersion heterogeneity.
      
      ------------------------------------------------------------------
       Method Estimate Std Error 99.9% CI       p-value F-stat
       PC-GMM    3.241     0.774   0.695, 5.786   0.000   47.3
      ------------------------------------------------------------------
      
      Overdispersion heterogeneity parameter estimate = 81.75673 
      
      Heterogeneity test statistic = 11.9284

