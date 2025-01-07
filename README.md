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

## Mapping to a Higher Dimension
+ [Click to view application for !D](https://www.bing.com/images/search?view=detailV2&ccid=Q%2f3fEto5&id=0724756F6C672379C7453228AA0665574CDCA9E5&thid=OIP.Q_3fEto5Fl6c9hvsHESnOgHaCK&mediaurl=https%3a%2f%2fwww.researchgate.net%2fprofile%2fNadhir_Ben_Halima%2fpublication%2f302594789%2ffigure%2fdownload%2ffig1%2fAS%3a360302345506818%401462914181636%2fMapping-from-1D-to-2D-Space-Feature-Space-for-Getting-Linearly-Separable-Data.png&cdnurl=https%3a%2f%2fth.bing.com%2fth%2fid%2fR.43fddf12da39165e9cf61bec1c44a73a%3frik%3d5ancTFdlBqooMg%26pid%3dImgRaw%26r%3d0&exph=248&expw=850&q=mapping+to+a+higher+dimensional+space+1D&simid=608043760946317765&FORM=IRPRST&ck=4B4987E225379026DB6E8C1966D4815E&selectedIndex=2&itb=0)

+ [Click to view Mapping for 2D](https://ibb.co/RNqHxNh)

## Projecting back to 2D after 2D was projected to 3D
[See diagram ](https://ibb.co/P486skx)

Note: Mapping to higher dimension is quite a complex computation, hence the kernel trick is used

## Kernel Trick

### What is the Kernel Trick?
_The kernel trick is a computational technique in machine learning, particularly in Support Vector Machines (SVMs) and other algorithms, that enables the model to perform calculations in a higher-dimensional feature space without explicitly transforming the data into that space. It computes the dot product of data points in the higher-dimensional space directly, using a kernel function._

### Why is the Kernel Trick Important?
+ Efficiency
> Explicitly transforming data into higher dimensions can be computationally expensive, especially for very high or infinite dimensions. The kernel trick avoids this by working directly with the dot product of the transformed data.

+ Handling Non-Linear Problems
> The kernel trick allows SVM (and other algorithms) to find decision boundaries for non-linearly separable data by implicitly mapping it to a space where it becomes linearly separable.

+ Flexibility
> Different kernel functions allow the algorithm to adapt to a variety of data distributions and relationships.
