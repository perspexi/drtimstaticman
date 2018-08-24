+++
### Date this page was created.
date = "2018-02-08"
### Project title.
title = "Audit: Linear Algebra"
slug = "audit_linalg"
draft = true
### Project summary to display on homepage.
summary = "Dalhousie Agricultural Campus [MTHA3000](https://academiccalendar.dal.ca/Catalog/ViewCatalog.aspx?pageid=viewcatalog&entitytype=CID&entitycode=MTHA+3000) Linear Algebra "
### Optional image to display on homepage (relative to `static/img/` folder).
image_preview = "cummingHall.jpg"
### Tags: can be used for filtering projects.
# Example: `tags = ["tag1", "tag2"]`
tags = ["course-audit"]
# Optional external URL for project (replaces project detail page).
external_link = ""
markup = "mmark"
# Does the project detail page use math formatting?
math = true
# Optional featured image (relative to `static/img/` folder).
[header]
image = "headers/linalgheadr.jpg"
caption = "Find Inverse of A :weary:"
###########################################################################
+++
# Jan 11, 2018 Lecture Notes
## Subscripts
### equations
[//]: # ( \begin{aligned}  )
[//]: # ( &nbsp;&nbsp;&nbsp;&nbsp;  )
$$a_{12} \quad x_1 \quad b_1  \qquad \Rightarrow \qquad a_{[eqn.  \#][ var. \#]} \quad x_{[var. \#]} \quad b_{[eqn.\#]}$$

$$AX=B \qquad \Rightarrow \qquad [matrix][coefficients] = [vector]$$
### matrices
$$
a_{[row][col]}
$$

$$
\begin{align}
\begin{bmatrix}
a_{11} & \dots & a_{1n} \\
\vdots & \ddots & \vdots \\
a_{m1} & \dots & a_{mn} \\
\end{bmatrix}
\end{align}
$$
+ $m$ is **rows**  ---  $n$ is **columns** how to remember?  
 - rows: upsidedown 'w' is 'm'  
 - columns: contains the letter n, also contains u, which is the upsidedown, mirror image of n.
+ A matrix element is generalized as $a_{ij}$ where $i =  1 \cdots m$ and $j =  1 \cdots n$
---
## Operations
Multiplication of two matrices:
Only multiply if $A_{m\times k}$ and $B_{k\times n}$. The product is $C_{m\times n}$
Therefore $AB \neq BA$. Note that $A(B+C)=AB+AC$  

How to multiply a matrix:
![matrix multiplicaiton](http://i.imgur.com/9aAiFcI.jpg)
Respective elements in the row and column are multiplied, (the row and column must have the same dimension) then all are added to yield the element in the new matrix.

> Written with [StackEdit](https://stackedit.io/).
