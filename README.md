# Early-LFA-Detection

This repository is about the "Edge-Assisted Label-Flipping Attack Detection in Federated Learning" paper which was published in IEEE Open Journal of the Communications Society

## Environment Setup

### Creating a Virtual Environment
This project uses a virtual environment named `EnvironmentName` to manage dependencies and ensure consistency across setups. The environment is specifically set up with Python 3.8 to support PyTorch 2.0.1 and CUDA 11.7, essential for running the experiments included in this project.

#### Steps to Create the Environment:
1. Open Anaconda Navigator.
2. Navigate to the 'Environments' tab.
3. Click on 'Create', enter the name `EnvironmentName`, and select Python 3.8 from the available options.
4. After the environment is created, activate `EnvironmentName` and open the terminal from within Anaconda Navigator.
5. Install the necessary dependencies to ensure compatibility with the project's requirements:
    ```bash
    conda install pytorch=2.0.1 torchvision torchaudio cudatoolkit=11.7 -c pytorch
    ```

### Configuring PyCharm
To utilize the `EnvironmentName` environment within PyCharm, follow these steps for integration:

1. Launch Anaconda Navigator.
2. Navigate to the 'Home' tab and ensure `EnvironmentName` is selected and activated from the environment dropdown menu.
3. Initiate PyCharm from Anaconda Navigator by clicking on the PyCharm icon.

### Running the Experiments
Once the environment setup is complete, you can run the experiments either through PyCharm or directly from your system's terminal.

#### Using PyCharm
1. Clone the repository:
    ```bash
    git clone https://github.com/nsmalotaibi/LFA-Detection.git
    ```
2. Open the cloned directory in PyCharm.
3. Check the interpreter settings in PyCharm to confirm that the `EnvironmentName` environment is selected as the Python interpreter.
4. Open the Terminal within PyCharm and run the following commands:
    ```bash
    python3 generate_default_models.py
    ```
    ```bash
    python3 label_flipping_attack.py
    ```

#### Using the Command Line
1. Ensure your `EnvironmentName` environment is activated:
    ```bash
    conda activate EnvironmentName
    ```
2. Navigate to the project directory:
    ```bash
    cd path/to/LFA-Detection
    ```
3. Run the scripts directly:
    ```bash
    python3 generate_default_models.py
    python3 label_flipping_attack.py
    ```

### General Information
- LFA hyperparameters can be set in the `label_flipping_attack.py` file.
- FL and experiment hyperparameters can be set in the `arguments.py` file.


## Citation
If you use this code, please cite the paper:
```
@article{alotaibi2024edge,
  title={Edge-Assisted Label-Flipping Attack Detection in Federated Learning},
  author={AlOtaibi, Nourah S and Felemban, Muhamad and Mahmood, Sajjad},
  journal={IEEE Open Journal of the Communications Society},
  year={2024},
  publisher={IEEE}
}
```


