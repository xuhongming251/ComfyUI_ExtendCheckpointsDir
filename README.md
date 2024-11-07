# ComfyUI: Extend Checkpoints Directory

Install this node to expand the directories for extra checkpoint models. You can add multiple directories.

## How to Use

1. Open the `__init__.py` file.
2. Modify it to include as many model folder paths as you need. For example:

   ```python
   folder_paths.add_model_folder_path("checkpoints", "G:/models/checkpoints")
   folder_paths.add_model_folder_path("checkpoints", "D:/ComfyUI/models/checkpoints")
   ```

3. After making these changes, restart your ComfyUI.

With this setup, the Load Checkpoint Node will be able to search for model files in all specified directories, such as `G:/models/checkpoints` and `D:/ComfyUI/models/checkpoints`.