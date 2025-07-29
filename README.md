# Load-Wash-Elute Simulation with CADET

This repository contains example simulations of a **Load-Wash-Elute** process using **CADET-Process** and **CADET-RDM**. A four-component system including `Salt` for the elution is simulated with a **Steric Mass Action** binding model and a **General rate model** unit operation model.
In **CADET-Process**, gradients can be used by either changing the concentration profile of an {class}`~CADETProcess.processModel.Inlet` (`lwe_concentration.py`) or by adding multiple inlets and dynamically adjusting their flow rates (`lwe_flow_rates.py`).


---

## Authors

* Johannes Schmölder
* Katharina Paul
* Ronald Jäpel
* Hannah Lanzrath

---

## Running the Example Simulation

1. Clone this repository.
2. Set up the environment using the `environment.yml` file.
3. Run the simulation:

   ```bash
   python main.py
   ```

The results will be stored in the `src` folder inside the `output` directory.

> **Note**: Running `cadet-rdm` requires [**Git LFS**](https://git-lfs.com/), which needs to be installed separately.
>
> * **Ubuntu/Debian**:
>
>   ```bash
>   sudo apt-get install git-lfs
>   git lfs install
>   ```
>
> * **macOS** (with Homebrew):
>
>   ```bash
>   brew install git-lfs
>   git lfs install
>   ```
>
> * **Windows**:
>   Download and install from [https://git-lfs.com](https://git-lfs.com)

---

## Output Repository

The output data for this case study can be found here:
[Link to Output Repository](https://github.com/cadet/RDM-Example-Load-Wash-Elute-Output)