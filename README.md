# MechaCar Statistical Analysis
## Linear Regression to Predict MPG

As per the results below, the coefficients vehicle_length and ground_clearance - not to mention the intercept - are statistically unlikely to provide random amounts of variance to the MPG values. 

Moreover, the slope of our linear model is not zero since the **p-value** of the linear model presents the value **_5.35e-11_**, even though this value is much smaller than the significance level of 0.05%.

According the summary results below, since the r-squared value is 0.71 it let us afirm that the linear regration model predicts mpg as the correlation among the variables is considerably high.

```
Call:
lm(formula = mpg ~ vehicle_length + vehicle_weight + spoiler_angle + 
    ground_clearance + AWD, data = mpg_Mechacar)

Residuals:
     Min       1Q   Median       3Q      Max 
-19.4701  -4.4994  -0.0692   5.4433  18.5849 

Coefficients:
                   Estimate Std. Error t value Pr(>|t|)    
(Intercept)      -1.040e+02  1.585e+01  -6.559 5.08e-08 ***
vehicle_length    6.267e+00  6.553e-01   9.563 2.60e-12 ***
vehicle_weight    1.245e-03  6.890e-04   1.807   0.0776 .  
spoiler_angle     6.877e-02  6.653e-02   1.034   0.3069    
ground_clearance  3.546e+00  5.412e-01   6.551 5.21e-08 ***
AWD              -3.411e+00  2.535e+00  -1.346   0.1852    
---
Signif. codes:  0 ‘***’ 0.001 ‘**’ 0.01 ‘*’ 0.05 ‘.’ 0.1 ‘ ’ 1

Residual standard error: 8.774 on 44 degrees of freedom
Multiple R-squared:  0.7149,	Adjusted R-squared:  0.6825 
F-statistic: 22.07 on 5 and 44 DF,  p-value: 5.35e-11
```

## Summary Statistics on Suspension Coils

According to the sumary tables below, it can be concluded that even though the total summary show a variance of only 69.29 pounds per square inch, the Manufactoring loc number 3 exceeds the 100 pounds per square inch dictated by design specifications for the MechaCar suspension coils' variance. The lot 3 presents variance of 170.29 pounds per square inch as per the results in the lot summary.

![image](https://user-images.githubusercontent.com/69650068/136680532-1f4f2a88-dc00-4027-8280-0776d332f79d.png)

![image](https://user-images.githubusercontent.com/69650068/136680549-3d81a147-e4de-4592-b12c-20a71573c1dd.png)

  
## T-Tests on Suspension Coils

Considering that the significance level is 0.05 percent, the p-value shown to all 4 results (all manufacturing lots and each lot individually) is above our significance level. Therefore, we do not have sufficient evidence to reject the null hypothesis, and we would state that the two means are statistically similar.

![image](https://user-images.githubusercontent.com/69650068/136682169-7404f80a-a967-4e96-a334-ab7820e4374d.png)


