# Use the devkitpro/devkita64 base image
FROM devkitpro/devkita64

# Update package list and install necessary packages
RUN apt update
# RUN apt install -y bear

# For arc
RUN apt install -y pip python-is-python3
RUN pip3 install requests

# For uScreen
RUN apt install -y maven

# For uDesigner
RUN git clone https://github.com/emscripten-core/emsdk.git
RUN /emsdk/emsdk install latest
RUN /emsdk/emsdk activate latest
RUN echo "source /emsdk/emsdk_env.sh" >> /root/.bashrc

# RUN dkp-pacman -Syu --noconfirm
