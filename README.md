# torch-test-xpu

## Description

Template for starting PyTorch projects with Intel GPUs (XPU) on Windows.

For more information, follow the official guide [here](https://pytorch.org/docs/stable/notes/get_start_xpu.html).

## Installation

1. Clone the repository:
   ```sh
   git clone <repository-url>
   cd torch-test-xpu
   ```

2. Set up the environment and install dependencies for PyTorch:

   **With pip:**
   ```sh
   python -m venv .venv
   pip install -r requirements.txt --extra-index-url "https://download.pytorch.org/whl/test/xpu"
   ```

   **With uv:**
   
   uv is an alternative to pip that is personally recommended. You need to install it first. See the [installation guide](https://docs.astral.sh/uv/getting-started/installation/).
   ```sh
   uv sync
   ```

3. PyTorch Prerequisites for Intel GPUs:

   Go to the [Intel guide](https://www.intel.com/content/www/us/en/developer/articles/tool/pytorch-prerequisites-for-intel-gpu/2-5.html), and follow the steps in the **Build for Intel Client GPUs > Install for Windows 10/11** section.

4. Additional Notes:

   Ensure you have Microsoft Visual Studio installed. The Intel Support Package will notify you if it's missing. Download Visual Studio from [here](https://visualstudio.microsoft.com/downloads/). For a lightweight option, on the same page, go to **All Downloads > Tools for Visual Studio**, and download the Build Tools for Visual Studio. Remember to set the Path variable.

   The oneAPI Environment script only works on CMD; it will not work on PowerShell.

## License

This project is licensed under the MIT License.