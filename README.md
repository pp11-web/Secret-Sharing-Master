# Secret Sharing Master

### Introduction
Secret Sharing Master is a Python-based application that implements a (k, n) threshold secret sharing scheme. In this scheme, a secret is divided into n shares, where only k or more shares can be combined to reconstruct the original secret. This application is built to ensure that sensitive data can be split among multiple participants in a secure way. Even if some participants are compromised, the secret remains protected until at least k valid shares are collected.

### Features
- Secret splitting: Split a secret into n shares using Shamir's Secret Sharing algorithm.
- Threshold reconstruction: Reconstruct the secret using any k out of n valid shares.
- Secure and efficient: Ensures the confidentiality of the secret and provides a simple, easy-to-use interface for both splitting and reconstruction.
- Customizable: Supports custom values for k (threshold) and n (total shares).
- Cross-platform: Works on any operating system with Python support.
### How It Works
Secret Sharing Master leverages Shamir's Secret Sharing algorithm, a cryptographic technique where:

- A secret is split into n shares.
- Any k or more shares can be used to reconstruct the secret.
- Fewer than k shares provide no information about the original secret.
The key idea is based on polynomial interpolation, where the secret is encoded as a constant in a randomly generated polynomial of degree k-1. Each share represents a point on this polynomial, and the secret can be reconstructed by solving the polynomial equation.
## Prerequisites
Before using the project, make sure you have the following installed:

- Python 3.x
- pip (Python package manager)
- Jupyter NoteBook.
- Anaconda Navigator.
All your files and folders are presented as a tree in the file explorer. You can switch from one to another by clicking a file in the tree.

### Installation
1. Clone the repository:
git clone https://github.com/pp11-web/Secret-Sharing-Master.git  
2. Navigate to the project directory:
cd Secret-Sharing-Master 
3. Install the required dependencies:
pip install -r requirements.txt
4. Run Project
Compile main.ipynb
### License
This project is licensed under the MIT License - see the LICENSE file for details.


### Acknowledgements
This project was inspired by the need for secure, easy-to-use secret sharing solutions. Special thanks to the cryptography community for providing the foundational algorithms used in this project.

