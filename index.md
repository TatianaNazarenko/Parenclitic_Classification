### Last Results (12.08.2020)
# Data: 
**266 proteins, 12 Controls, 37 Cases**
# Model
- Internal (for each pair of proteins): radial SVM (crossvalidation) - weights of connection = probability to beloning class 1
```markdown
svmFit <- train(Group ~ p1 + p2 + **AGE**,
                  data = data, method = _"svmRadial"_, preProc = c("center", "scale"),metric = "ROC",
                  trControl = trainControl(method = **"cv"**, classProbs = TRUE, summaryFunction = twoClassSummary))
```
                                           
- External (for network characterisitcs): glm (LOOCV)
```markdown
glmFit <- train(Group ~ _1 network characterisitc_,
                  data = df_train, method = _"glm"_, preProc = c("center", "scale"), metric = "ROC",
                  trControl = trainControl(method = **"LOOCV"**, classProbs = TRUE, summaryFunction = twoClassSummary))
```
# Main results
Right side plots: Each model is built on only one characteristic
![Image](FINAL_FIG_FULL.jpg)
## Can we reduce number of proteins?
![Image](SELECT_EDGES.jpg)
![Image](HIST_FREQ.jpg)
![Image](BAR.jpg)
## Results of Parenclitic only on 13 proteins
![Image](FINAL_FIG_SMALL.jpg)
### Networks
![Image](NETWORKS.PNG)
## Results of Parenclitic (WITHOUT AGE) only on 13 proteins (the same)
![Image](FINAL_FIG_SMALL_WA.PNG)


You can use the [editor on GitHub](https://github.com/TatianaNazarenko/Parenclitic_Classification/edit/master/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/TatianaNazarenko/Parenclitic_Classification/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
