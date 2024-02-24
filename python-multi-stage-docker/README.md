# Python Multi-Stage Docker Build

This project demonstrates how to use multi-stage Docker builds to create a lightweight Docker image for a simple Python application. The application consists of a Python script that performs addition of two numbers.

## Files

- addition.py: Contains a Python script with a function to add two numbers.
- Dockerfile_single: Single-stage Dockerfile to build the Docker image using a Python base image.
- Dockerfile_multi: Multi-stage Dockerfile to build the Docker image using distroless image for reduced size.
- README.md: This file, providing an overview of the project and instructions for usage.

## Usage

1. *Single-Stage Build*:
   - Build the Docker image using the single-stage Dockerfile:
     bash
     docker build -t python-addition-single -f Dockerfile_single .
     
   - Run the Docker container:
     bash
     docker run python-addition-single
     

2. *Multi-Stage Build*:
   - Build the Docker image using the multi-stage Dockerfile:
     bash
     docker build -t python-addition-multi -f Dockerfile_multi .
     
   - Run the Docker container:
     bash
     docker run python-addition-multi
     

## Conclusion

By comparing the sizes of the resulting Docker images from single-stage and multi-stage builds, you'll observe a reduction in image size achieved by using multi-stage builds and distroless images.

## Contributing

Contributions are welcome! Feel free to submit pull requests with improvements or additional features.

## License

This project is licensed under the [MIT License](LICENSE).
