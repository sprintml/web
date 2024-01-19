---
layout: post
title:  "76 days to go: How to submit your paper to ArXiv?"
date:   2023-06-18
tags: phd life, research, arxiv submission
---

*by Adam Dziedzic and Franziska Boenisch*

A paper is more than a research idea and experiments, unfortunately. You also have to give talks about your research, publish your code, paper, and promote your work. In this post, we focus on the bread-and-butter of ML researchers, namely, on "how to submit your paper to ArXiv?". 

First of all, we assume that you have your paper in the LaTex format on overleaf. Before publishing, you might also want to first add the authors (since the submission is often double-blinded), their affiliations, then you can add ackonwledgements, pointer to your code, etc. Next, download your files as a zip file and then use the cleaning tool to remove all the comments. This is an important step since you might not want to publish the work on ArXiv that someone else can get the LaTex source of and see all your comments, previous versions of your paragraphs, etc. If this is not desirable, and even more, this is not intended to be read by anoone else, then use the [arxiv-latex-cleaner tool](https://github.com/google-research/arxiv-latex-cleaner). Our favorite command is simply ```arxiv-latex-cleaner --keep_bib folder_from_overleaf```. Then, copy to a different location and rename the produced folder to the original name (to preserve the references from LaTex). If your figure files or images were deleted from the cleaned version, simply add the images from the original version. You might also select which images you want to publish but double check that all images referenced in the text are present in the folder for figures. 

Once you clean the LaTex files, simply zip them, and upload to overleaf as a new project. Then, compile the whole document again from scratch to check that there are no missing references or images. Once everything is correct, go to the top-right menu on overleaf, click Submit, and select 'submit your paper to ArXiv'. Choose 'Download project ZIP with submission files (e.g., bbl) and save it on disk. Unzip the folder locally on your machine, move the .bbl file to the main folder where the whole project is. Zip the whole project.

Now, you are ready to submit your paper to arXiv. Login there, select 'Submit New Submission', check all the necssary boxes, you can select 'arXiv.org perpetual, non-exclusive license', and the primary classifiation as Computer Science -> Machine Learning. Then click on continue, browse to find the zipped folder, and upload files. Continue to process the files. If everything is correct add the metadata (author, title, abstract, and indiate in the comments, e.g., ```Accepted at NeurIPS2024``` if this is the case, or any other comment that you find would be useful for the readers).

Finally, share with your colleagues the URL to the submission. Hope that your paper can be easily accessible to other researchers and they can benefit from your contributions. In the next posts, we will also talk more on how to prepare a code for submission and provide you with more useful tips on how to publish your work.