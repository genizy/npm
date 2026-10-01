# How to deploy your own

Before starting, install **Git**, **Python**, and **Node.js (with npm)**.

1. **Clone the repository** and open its folder:
   ```bash
   git clone https://github.com/genizy/npm
   cd npm
   ```

2. **Prepare the files:**
   - Delete the `gnrunner` folder.
   - Move everything inside `deploy-your-own` into the repository’s root folder.

3. **Set your package name.** Open `RUN.py` and replace:
   ```python
   name = "tuffname"
   ```
   with the npm package name you want to use.

   Use an existing package you have permission to publish, or choose an available name for a new package. If you’re new to npm, [create an account](https://www.npmjs.com/signup) and follow the [official publishing tutorial](https://docs.npmjs.com/creating-and-publishing-unscoped-public-packages/).

4. **Run the setup script:**
   ```bash
   python RUN.py
   ```
   If your system uses `python3`, run `python3 RUN.py` instead.

5. **Delete `RUN.py`** after the script finishes successfully.

6. **Sign in to npm and publish** from the repository’s root folder:
   ```bash
   npm login
   npm publish
   ```
   Follow any authentication prompts.

Once publishing succeeds, your package will be available at `https://www.npmjs.com/package/YOUR-PACKAGE-NAME`.