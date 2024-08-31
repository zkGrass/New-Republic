Backend code for new-repulic protocol.
Started at August 20 2024.
Expected to launch at October 8 2024

### Preview
Explanation of Parameters
CUDA_VISIBLE_DEVICES=0: Specifies which GPU to use. 0 indicates the first GPU. Adjust this based on your available GPUs.
--hf_token: Your Hugging Face token, required for accessing certain models. This should token should have write access.
--flock_api_key: Your FLock API key.
--task_id: The ID of the task you want to validate. If you are validating multiple tasks, you can pass a list eg. if you are validating tasks 8 and 9, you can pass --task_id 8,9
--validation_args_file: The path to the validation arguments file.
--auto_clean_cache: A flag to determine whether to automatically clean the model cache.
--lora_only: A flag to indicate whether to validate only repositories with LoRA (Low-Rank Adaptation) weights. True means only LoRA weights will be validated. This is useful for validators with limited network bandwidth, as LoRA weights are significantly smaller (10-500 MiB) compared to full model files (>10 GiB).
