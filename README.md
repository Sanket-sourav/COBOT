# COBOT - SmolVLA checkpoint

Fine-tuned SmolVLA policy for the MuJoCo cobot simulation.

## Download

[Latest model checkpoint](https://github.com/Sanket-sourav/COBOT/releases/tag/smolvla-1321-5341-step-1000)

Run: `cobot_smolvla_1321_5341` - training step **1000**.
The release ZIP includes weights, model configuration, tokenizer, processors, normalization data, saved training configuration, a manifest, and upstream attribution/license files.

Download and extract the ZIP, then select its `pretrained_model` folder in `run_policy.py`.

## Model inputs and outputs

- Images: wrist RGB and fixed RGB.
- State: six measured joint angles in radians and gripper closure percentage.
- Actions: six absolute joint targets in radians and gripper closure (0 open, 100 closed).

Base model: [lerobot/smolvla_base](https://huggingface.co/lerobot/smolvla_base).
The upstream model declares Apache-2.0; its license and attribution are included in the release archive.

Archive SHA-256: `11064e85840822fb96c645c742b4dec782eeb16fa980726666bddfdb1a86966e`.
