trtexec \
--onnx=feature_booster_explicit.onnx \
--saveEngine=feature_booster_fp16.engine \
--fp16 \
--memPoolSize=workspace:4096 \
--profile=0 \
--minShapes=descriptors:1x1x256,keypoints:1x1x4 \
--optShapes=descriptors:1x4000x256,keypoints:1x4000x4 \
--maxShapes=descriptors:1x8000x256,keypoints:1x8000x4
