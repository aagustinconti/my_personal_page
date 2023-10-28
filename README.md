# How I Built This Website

## Repository

1. I created the basic PUBLIC repository on GitHub with a README file, a .gitignore file, and MIT License.
2. I cloned that repository to my local machine using the following command:

    ```sh
    git clone <name-of-my-repo>
    ```

## Virtual Environment

3. I set up a virtual environment using [Poetry](https://python-poetry.org/docs/basic-usage/):

   ```sh
   poetry init
   poetry add mkdocs
   poetry add mkdocs-material
   poetry add mkdocs-material-extensions
   ```

## Mkdocs

4. Initialized the mkdocs files with the following command:

    ```sh
    poetry run mkdocs new .
    ```

5. Created a new page named `downloads.md` in the `/docs` directory.

6. Edited the configuration file `mkdocs.yaml` to include the following:

    a. `site_url`
    b. `repo_url`
    c. `repo_name`
    d. `favicon`
    e. `logo`
    f. `icon/repo`
    g. `extra/analytics`

    For more details, refer to the [Mkdocs Material Documentation]().

7. Tested all the changes using:

    ```sh
    poetry run mkdocs serve
    ```

## GitHub Pages

8. Created the `.github/workflows/ci.yaml` file following the instructions in [Mkdocs Material Documentation](https://squidfunk.github.io/mkdocs-material/publishing-your-site/).

9. Pushed all the changes using the commands:

    ```sh
    git add --all
    git push origin main
    ```

10. Configured the GitHub Page as shown in the image below:

![GitHub Pages Configuration](/docs/source/images/github-pages-config.png)

# Online Test

11. Accessed the page using the original link:

![Online Test](/docs/source/images/working-test.png)

## References

- [How To Create STUNNING Code Documentation With MkDocs Material Theme - YouTube Video](https://www.youtube.com/watch?v=Q-YA_dA8C20&t)
- [Mkdocs material](https://squidfunk.github.io/mkdocs-material/getting-started/)
- [Poetry](https://python-poetry.org/docs/basic-usage/)
