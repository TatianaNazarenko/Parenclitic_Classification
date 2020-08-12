### Last Results (12.08.2020)
# Data: 
**266 proteins, 12 Controls, 37 Cases**
# Model:
- Internal (for each pair of proteins p1 and p2): radial SVM (crossvalidation) - weights of connection = probability to beloning class 1
```markdown
svmFit <- train(Group ~ p1 + p2 (or + AGE),
                  data = data, method = "svmRadial", preProc = c("center", "scale"),metric = "ROC",
                  trControl = trainControl(method = "cv", classProbs = TRUE, summaryFunction = twoClassSummary))
```
                                           
- External (for network characterisitcs): glm (LOOCV)
```markdown
glmFit <- train(Group ~ (1 network characterisitc),
                  data = df_train, method = "glm", preProc = c("center", "scale"), metric = "ROC",
                  trControl = trainControl(method = "LOOCV", classProbs = TRUE, summaryFunction = twoClassSummary))
```
# Results (Parenclitic WITH Age) 
_**35 245 edges** ~15 hours_

![Image](FINAL_FIG_FULL.jpg)
## Can we reduce number of proteins?
For each edge calculate avarage "weight" for 0-group and avarage "weight" for 1-group
![Image](SELECT_EDGES.jpg)
Looks like "red cloud" <- pairs of proteins where SVM didn't find solution (I think these guys were the ones who spoiled the previous models).

Calculation of how often each protein is found in the blue cloud (we think that if a protein is significant, then it will be found there more often, that is, the better other pairs with it will distinguish between groups).
![Image](HIST_FREQ.jpg)

I selected only those proteins if the number of their connections that got into the blue cloud is more than half of all proteins.
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
