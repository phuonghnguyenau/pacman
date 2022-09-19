FROM registry.access.redhat.com/ubi8/nodejs-16-minimal:1-65

LABEL org.opencontainers.image.authors="Ivan Font (Original) <ifont@redhat.com>, Phuong Nguyen (Modifications) <pnguyen@redhat.com>"

# Create app directory
RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

# Clone game source code
RUN git clone https://github.com/phuonghnguyenau/pacman.git .

# Install app dependencies
RUN npm install

# Expose port 8080
EXPOSE 8080

# Run container
CMD ["npm", "start"]
