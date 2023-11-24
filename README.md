# Problem Sets 5 and 6

In Problem Set 5 we will be exploring n-grams, collocations, and a new measure of word importance, TF-IDF.

In Problem Set 6, using some of the same data, we will build word2vec models, compare those models to a large word2vec model, and explore using sentence embeddings.

Remember that I drop your lowest problem set score! If you've done well on the first four problem sets, you can skip either PS5 or PS6 and have the one you skip be the one I drop.

Both problem sets are due Monday, November 27, at 11:59pm EST. Exact requirements for submission can be found at the end of this page.

## Preparing the data for both problem sets
You will need to get some data that you'll use for both PS5 and PS6. You will complete this step once and use the data for both problem sets, which are linked to below.

For problem set 4, you [wrote a nice Python script](https://github.com/CSCI-2349-F23/ps4#part-2-getting-the-text-for-a-particular-category-page) that got all the pages on a Wikipedia category page and saved the text on each page to a string in a list of strings, removing stuff in brackets and replacing all new lines with space.

For PS5 and PS6, you will rewrite your script so that instead of saving each page's text to a string in a list of strings, it **writes each page's text to a separate `.txt` file whose name corresponds to the title of that page**. All `.txt` files for a particular category will be stored in a directory whose name corresponds to the title of that category. You can create that directory manually before you run your script, or you can include code for creating that directory in your script.

Call your script `get_text.py` and place it in this directory. Then run it on **one of the three Wikipeda category pages** you used for PS4. Pick a category with **at least 50 pages** and with **articles that are long**. Make sure to use **real Wikipedia** and not simplified Wikipedia.

If you did not successfully complete PS4, you can use the code I provide in the solution, which is found attached the Assignment in Canvas for PS4. Keep in mind that you will have to edit it to create text files rather than saving the text to a list of strings.

Here's what my directory structure looks like after I run my version of the script on the [Endangered Animals category page](https://en.wikipedia.org/wiki/Category:Endangered_animals).

```
emilypx@Yodi ps5and6 % ls -1
Endangered_animals
README
all19thcent.txt
allcontempo.txt
get_text.py
ps5.ipynb
```

And here's what it looks like when I `ls` the `Endangered_animals` directory:

```
emilypx@Yodi ps5and6 % ls Endangered_animals/ | head -10
African_bush_elephant.txt
Al_Houbara_Protected_Area.txt
Anacropora_spinosa.txt
Anapistula_seychellensis.txt
Anatemnus_seychellesensis.txt
Andean_mountain_cat.txt
Anepsiozomus_sobrinus.txt
Anodonta_pseudodopsis.txt
Ansell%27s_shrew.txt
Anthicus_sacramento.txt
```

---

## Problem Set 5
To complete PS5, launch Jupyter notebook and open `ps5.ipynb`. You should do this on your own machine. If you skipped PS4, go back and follow the [directions in PS4 for making sure you have all right libraries installed](https://github.com/CSCI-2349-F23/ps4#part-0-installing-libraries). You will complete the problem set in the notebook.

---

## Problem Set 6
You will complete PS6 on Google Colab. [Follow this link](https://colab.research.google.com/drive/15bNO-v_zua-4rbhqOv2yNt-9gBXeUDaL?usp=sharing) to the Colab file called `ps6.ipynb`, and then follow the directions in the Colab file to make your own copy of the file in your Google Drive. Then continue to follow the directions and complete the assignment.

---

## What to submit
1. Download your completed `ps6.ipynb` from Colab to this directory.
2. Make sure you have these items in this directory *plus* your directory full of Wikipedia text that you created in Step 1, above.
```
allcontempo.txt
all19thcent.txt.
get_text.py
ps5.ipynb
ps6.ipynb
README
```
Note: If you chose to do only one of the two problem sets, only include that `pynb` file in your submission.

3. Tar and zip up the directory, calling it `ps5and6.tgz`.
4. Upload that file to Canvas. If you are completing both problem sets, submit the same `.tgz` to both assignments on Canvas. If you are only completing one problem, upload the `.tgz` file only to the assignment you are completing.

These assignments are due November 27 at 11:59pm EST.

