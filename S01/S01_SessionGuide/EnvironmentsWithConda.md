# Creating and using environments with `conda`

Anaconda environments allow you to manage separate sets of packages and their dependencies for different projects. This can be useful if you need to use different versions of packages or if you want to keep your global package set clean.

Here are some common tasks for working with environments in Anaconda:

1. **Creating an environment:** To create a new environment called myenv, use the following command:

   ```bash
   conda create --name myenv
   ```

    You can also specify which packages you want to include in the environment by adding them to the command:

    ```bash
    conda create --name myenv numpy scipy pandas
    ```

2. **Activating an environment:** To activate an environment, use the following command:

    ```bash
    conda activate myenv
    ```

3. **Deactivating an environment:** To deactivate the current environment, use the following command:

    ```bash
    conda deactivate
    ```

4. **Listing environments:** To list all of the environments you have created, use the following command:

    ```bash
    conda env list
    ```

5. **Removing an environment:** To remove an environment called myenv, use the following command:

    ```bash
    conda env remove --name myenv
    ```

6. **Installing packages in an environment:** To install a package in a specific environment, activate the environment first, then use the conda install command:

    ```bash
    conda activate myenv
    conda install scikit-learn
    ```

    Sometimes the package is not available in the default channel, so you need to specify the channel where it is available. For example, to install the package from the `conda-forge` channel, use the following command:

    ```bash
    conda install -c conda-forge scikit-learn
    ```


7. **Exporting an environment:** To export a list of the packages in an environment to a requirements.txt file, use the following command:

    ```bash
    conda list --explicit > requirements.txt
    ```

8. **Creating an environment from a file:** To create a new environment from a requirements.txt file, use the following command:

    ```bash
    conda create --name myenv --file requirements.txt
    ```
