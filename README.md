# Kernel_SVM

## Kernel Support Vector Machine (Kernel SVM)
_Kernel SVM is an extension of the standard Support Vector Machine that uses kernel functions to handle non-linear decision boundaries. It allows SVM to work in cases where the data is not linearly separable in its original feature space by projecting it into a higher-dimensional space._

## Why Kernel SVM?
> + Standard SVM can only draw linear hyperplanes, which limits its use for linearly separable data.
> + Kernel SVM enables the algorithm to find a decision boundary in higher dimensions without explicitly computing new features, making it efficient and powerful for non-linear problems.

## Kernel Use
It is good for non linearly separable data.
+ [Click to view separable and non separable data](https://www.bing.com/images/search?view=detailV2&ccid=aYSDuNl6&id=6F3C2D25D4C7FF57E483F9DBB90B97071DFC2D97&thid=OIP.aYSDuNl6u06o5zqAA4ISBQHaCv&mediaurl=https%3a%2f%2fvitalflux.com%2fwp-content%2fuploads%2f2022%2f04%2fLinearly-vs-Not-linearly-separable-datasets.png&cdnurl=https%3a%2f%2fth.bing.com%2fth%2fid%2fR.698483b8d97abb4ea8e73a8003821205%3frik%3dly38HQeXC7nb%252bQ%26pid%3dImgRaw%26r%3d0&exph=363&expw=979&q=linear+separable+and+non+linear+separable&simid=608009933807172416&FORM=IRPRST&ck=055DB1A1545FD51E468A5EF7E8762EBC&selectedIndex=0&itb=0)

## What is a Higher-Dimensional Space in Machine Learning?
_In machine learning, a higher-dimensional space refers to a space with more features or dimensions than the original input space. This is often done to make data that is not linearly separable in its original space separable by mapping it to a space where a linear hyperplane can effectively classify the data._


## What is a Higher-Dimensional Space in Machine Learning?
_In machine learning, a higher-dimensional space refers to a space with more features or dimensions than the original input space. This is often done to make data that is not linearly separable in its original space separable by mapping it to a space where a linear hyperplane can effectively classify the data._

### Why Use a Higher-Dimensional Space?
_Some datasets are non-linearly separable in their current form, meaning no straight line (or hyperplane) can divide the classes. By projecting the data into a higher-dimensional space:_

+ Linear Separability: The algorithm can find a hyperplane in the transformed space that separates the classes.
+ Feature Relationships: Non-linear relationships between features in the lower-dimensional space become linear in the higher-dimensional space.
