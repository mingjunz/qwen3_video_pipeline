View it at: https://mingjunz.github.io/qwen3_video_pipeline/

Architecture Overview — How Qwen3VL transforms raw video frames into vision tokens for multimodal language models.
This document walks through the 7-step pipeline that converts a 30-frame video into 192 vision tokens /embedding features(3584-d each). The pipeline handles frame sampling, spatial resizing, patch extraction, temporal pooling, token serialization, and vision encoding — producing the feature embeddings consumed by the transformer backbone.
Key parameters: patch_size=16, merge_size=2, temporal_patch_size=2, grid=8×8, vision_dim=3584

