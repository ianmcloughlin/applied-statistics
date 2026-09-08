# Assessment Brief: Applied Statistics, Winter 26/27

This assessment gives you an opportunity to show your achievement of the module learning outcomes.
The main part of the assessment is to complete the problems in the [Problems](#problems) section of this document.
Start by making a new GitHub repository solely for this assessment.
Create a new Jupyter notebook named `problems.ipynb` in the root of the repository.
Create a file called [`AGENTS.md`](https://realpython.com/agents-md/) in the root of your repository and copy [the contents of the example agents file in the notes section of this repo into it.](notes/example-agents.md?plain=1)
Submit the repository URL using the link below before the URL submission date.
You should then work consistently on your repository until the final deadline for commits below.
The last commit pushed to GitHub on or before the deadline will be assessed.

> [!IMPORTANT]
> [Submit Your Repository URL Here by 30 September 2026 (ATU Login required)]()  
> 
> Final Deadline for Commits:  
> <ins>**20 December 2026**</ins>  

Always keep your latest work in GitHub.
If you have problems, especially with git, ask for help well before the deadline.
Do not delete your repository without consulting the lecturer.
Disproportionately large commits, especially near the final deadline, will usually not be accepted.
Make sure to consult and adhere to the policies on the student portal, such as those relating to student conduct and plagiarism.

## Target Audience

Complete the assessment with the following target audience in mind: an informed computing professional, such as a prospective employer.
Assume they have a strong background in computing but may not be familiar with the specific language, packages, or tools you use.
They should be able to clone your repository and run any code within it with minimal setup and without any extra help from you.
Include setup instructions in your `README.md`, and keep all necessary data files and images cleanly organized.
If any files are too large to include in your repository, explain this in your `README.md` and, where possible, provide code to automatically download them.

## Organization and Structure

Your submission should be in the `main` branch of your repository.
Include a clear [`README.md`](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes), a suitable [`.gitignore` file](https://www.toptal.com/developers/gitignore), and an [accurate `requirements.txt` file](https://realpython.com/what-is-pip/#using-requirements-files).
Avoid including [unnecessary files or folders](https://realpython.com/python-git-github-intro/#what-not-to-add-to-a-git-repo).
Use lowercase file and folder names, except for the usual files like `README.md`.
Do not use spaces or special characters in filenames.
Underscores, hyphens, and full stops are okay.

Your commit history should show how your work evolved: improvements, refinements, and added clarity.
Keep your notebook [reproducible, clean, and concise.](https://arxiv.org/pdf/2202.07233)
Use a [level 1 heading](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#headings) for the notebook title.
Use [level 2 Markdown headings](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#headings) to clearly identify each problem within the notebook.
Use Markdown cells to give explanations and insights into your code.

Follow Python coding standards and guidelines such as [PEP8](https://peps.python.org/pep-0008/).
Write clean, readable, and efficient code using meaningful variable names and consistent formatting.
Break code into smaller, manageable cells whenever possible.
Each code cell should focus on a single step in your overall solution.
Include [meaningful comments](https://realpython.com/python-comments-guide/) and [docstrings](https://peps.python.org/pep-0008/#documentation-strings) in your code.
You can use [modules in the standard library](https://en.wikipedia.org/wiki/Standard_library) and any of the packages in the [requirements.txt file in this repository](./requirements.txt) and their dependencies.
Ask before using anything else.

## Submission Checklist

- [ ] **Repository Link Submitted:** You have submitted your GitHub repository URL in the format `https://github.com/username/reponame` via the Microsoft Forms link above.

- [ ] **Agents file included from the start:** You have had the correct `AGENTS.md` in the root of your repository from the start.

- [ ] **Correct Notebook Name:** Your primary submission file is located in the root of the repository and is named exactly `problems.ipynb` (all lowercase, no spaces).

- [ ] **Essential Files:** Your repository includes a `.gitignore`, a `README.md` with setup instructions, and a `requirements.txt` listing all necessary Python packages (e.g., `numpy`).

- [ ] **Notebook Cell Order:** You have restarted the kernel and run all cells in your notebook to ensure they execute in sequential order (1, 2, 3...) without errors, providing a clean and reproducible output.

- [ ] **Folder Organization:** Any extra files are organized into subfolders; specifically, any datasets are in a `/data` folder and any images, plots, or diagrams are in an `/img` folder.

- [ ] **Repository Tidiness:** You have removed all irrelevant files (e.g., `.DS_Store`, `__pycache__`, local checkpoints, or temporary scratchpads).

- [ ] **Environment Reproducibility:** When someone clones your repo, they will likely use the following workflow. Ensure your `README.md` and `requirements.txt` make this process seamless:

    1. `git clone <repo-url>`
    2. `pip install -r requirements.txt`
    3. `jupyter notebook problems.ipynb`

## Marking Scheme

Your submission will be assessed across the following five equally-weighted categories.
Make sure you provide clear evidence within your repository of the criteria listed.
A good submission will meet most of the criteria in each category.
An excellent submission will demonstrably meet all the criteria.
Note that the overall impression your submission makes may influence marks in each category.

### Presentation

- Your repository should be well-organized, with a clear and logical structure.
- Your `README.md` should clearly explain the purpose of your repository and how to run any code it contains.
- Your notebook should present a clear narrative, making it easy to follow your thought process.
- A knowledgeable expert reviewing your repository should be able to understand its contents without your help.

### Research

- Your submission should demonstrate research on relevant topics, showing an understanding of the material.
- You should build upon existing literature and documentation rather than just presenting basic solutions.
- References and comparisons to similar work should be included.
- References should be put into context - how and why they are relevant to your submission.

### Documentation

- Your repository should contain standard files, such as a `README.md`, to provide context for your work.
- All concepts should be clearly and concisely explained within your notebooks.
- Code should include informative comments that clarify its purpose and functionality.
- Your `README.md` and notebook should have clear headings and provide a clear context for their contents.

### Development

- Your code should be efficient and well-structured, effectively addressing the problem at hand.
- Standard programming structures, algorithms, and testing methods should be applied where appropriate.
- The overall architecture of your code should be clean, demonstrating good coding practices.
- Your code should demonstrate your knowledge of established style conventions and norms.

### Consistency

- Each commit should focus clearly on a single unit of work.
- Your commit history should show consistent activity across the assessment period, not a burst of late submissions.
- Your repository should demonstrate incremental review and refinement rather than one-off completion.
- Commits should capture improvements to both code quality and explanations over time.

## Problems

Complete all problems below in your `problems.ipynb` notebook.
Your notebook should tell a story, using Markdown cells to explain your thinking and code cells to perform the technical tasks.
Your notebook must also run from top to bottom on a standard machine in three minutes or less.

### Problem 1: Exploring Petal Length

The [Iris dataset](https://raw.githubusercontent.com/mwaskom/seaborn-data/master/iris.csv) contains measurements of 150 iris flowers belonging to three species: `setosa`, `versicolor`, and `virginica`.
For each flower, the dataset records sepal length, sepal width, petal length, and petal width.

Using the Iris dataset, investigate the distribution of `petal_length`.

1. Plot a histogram showing the petal lengths of all 150 flowers.
2. On the same plot, superimpose an appropriate normal distribution, using the mean and standard deviation calculated from the data.
3. Create separate histograms for each of the three species, and superimpose an appropriate normal distribution on each.
4. Report the mean and standard deviation of petal length for the complete dataset and for each species.
5. Describe and compare the distributions you observe. In particular, discuss whether a normal distribution appears to be a reasonable model for petal length overall and within each species.

### Problem 2: Correlation Between Petal Length and Petal Width

Investigate the relationship between `petal_length` and `petal_width` in the Iris dataset.

1. Calculate the Pearson correlation coefficient between petal length and petal width using all 150 flowers.
2. Create an appropriate scatter plot showing the relationship between the two variables, and include a suitable line to help illustrate the relationship.
3. Calculate the Pearson correlation coefficient separately for each of the three species.
4. Create an appropriate plot showing the relationship between petal length and petal width for each species.
5. Report and compare the correlation coefficients.
6. Explain what the correlation coefficients tell you about the relationship between petal length and petal width, both for the dataset as a whole and within each species.

### Problem 3: Comparing Species Using t-Tests

Investigate whether the three iris species differ in their `petal_length` and `petal_width`.

For each pair of species:

- `setosa` vs `versicolor`
- `setosa` vs `virginica`
- `versicolor` vs `virginica`

perform an independent-samples t-test for:

- petal length,
- petal width.

For each test:

1. State the null and alternative hypotheses.
2. Calculate the t-statistic and p-value using `scipy.stats`.
3. Use a significance level of $\alpha=0.05$ to decide whether to reject the null hypothesis.
4. Summarise your results in an appropriate table.
5. Explain what the results tell you about differences between the three species.

### Problem 4: Comparing the Species Using ANOVA

The t-tests in Problem 3 require several separate comparisons between species.
Instead, investigate differences in **petal length** and **petal width** using one-way analysis of variance (ANOVA).

For each variable:

1. State the null and alternative hypotheses for a one-way ANOVA.
2. Perform a one-way ANOVA comparing the three species using `scipy.stats`.
3. Report the F-statistic and p-value.
4. Use a significance level of $\alpha=0.05$ to determine whether there is evidence that the species have different population means.
5. Explain what the ANOVA result tells you and what it does not tell you about the individual species.

The t-tests in Problem 3 involved three pairwise comparisons. Explain why performing several separate hypothesis tests can increase the overall probability of making a type I error, and explain how ANOVA addresses this problem by testing the three group means simultaneously.

Finally, compare the conclusions from your t-tests with those from the ANOVA and explain why ANOVA is generally preferable when comparing more than two groups.


***

**End**
