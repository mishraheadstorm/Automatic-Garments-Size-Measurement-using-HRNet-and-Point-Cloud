# Notes

- 4/30 change: Changed the requirements.txt file. With the docker file, the numpy version and the opencv versions were not compatible. Adjusted them to latest, but may have to update some of the source code
- 4/30 change: docker file is debian bulls eye, and needs the nvcc (nvidia cuda libraries) to compile the model ( may be very difficult on a mac with M1 chip, this would need to be moved to Metal instead of cuda)
- 5/2 change: setup the nms library to build without CUDA support. This should enable processing via Mac or other CPU only hardware.