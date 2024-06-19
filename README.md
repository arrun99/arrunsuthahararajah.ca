# My Resume Website

Welcome to the repository for my personal resume website, hosted on Google Cloud. This website showcases my professional background, skills, and achievements. It is designed with simplicity and speed in mind, leveraging several Google Cloud services to ensure optimal performance and availability.

## Website Overview

The website is hosted on Google Cloud and includes the following components:
- **HTML/CSS**: The structure and styling of the website.
- **Images**: Visual content that complements the resume information.
- **Resume File**: A downloadable version of my resume in PDF format.

## Hosting and Configuration

### Google Cloud Storage

All website files, including HTML, CSS, images, and the resume file, are stored in a Google Cloud Storage bucket. This ensures reliable and scalable storage with high availability.

### Load Balancer

A Google Cloud Load Balancer manages incoming traffic to the website. The load balancer distributes requests to the Google Cloud Storage bucket, ensuring efficient and reliable access.

### Domain and DNS Configuration

The website is accessible via a fully qualified domain name (FQDN). The domain's DNS server is configured with an "A" record that points to the public IP address of the load balancer, resolving the FQDN to the correct IP.

### Cloud CDN

Google Cloud's Content Delivery Network (CDN) is enabled to cache website content. This significantly improves load times for users by serving cached content from locations closer to them.

## Repository Structure

```
.
├── index.html
├── styles/
│   └── main.css
├── assets/
│   ├── images/
│   │   └── profile.jpg
│   └── resume.pdf
└── README.md
```

- `index.html`: The main HTML file for the website.
- `styles/`: Directory containing CSS files for styling the website.
- `assets/`: Directory containing images and resume file.
  - `images/`: Directory containing image files used on the website.
  - `resume.pdf`: The resume PDF file.
- `README.md`: This README file.

## Getting Started

To view the website, simply navigate to the following URL: [arrunsuthahararajah.ca](https://arrunsuthahararajah.ca/)

If you would like to replicate this setup or contribute to the project, follow these steps:

### Prerequisites

- Google Cloud Platform Account
- Domain Name

### Steps

1. **Clone the Repository**
   ```bash
   git clone https://github.com/arrun99/arrunsuthahararajah.ca.git
   cd arrunsuthahararajah.ca
   ```

2. **Upload Files to Google Cloud Storage**
   - Create a Google Cloud Storage bucket.
   - Upload the `index.html`, `styles/`, and `assets/` directories to the bucket.

3. **Set Up Load Balancer**
   - Create a new load balancer in the Google Cloud Console.
   - Configure the load balancer to point to your Google Cloud Storage bucket.

4. **Configure DNS**
   - Update your domain's DNS settings to add an "A" record.
   - Point the "A" record to the public IP address of your load balancer.

5. **Enable Cloud CDN**
   - Enable Cloud CDN for your load balancer to cache website content.

## Template Acknowledgment

The HTML/CSS template for this website is based on the [Digital Resume](https://github.com/divanov11/Digital-Resume) repository by [divanov11](https://github.com/divanov11). I adapted and customized it to fit my personal resume and design preferences.

## Contributions

Contributions to improve the website are welcome. Feel free to open issues or submit pull requests.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

Thank you for visiting my resume website repository!

[![Visits Badge](https://badges.pufler.dev/visits/arrun99/arrunsuthahararajah.ca)](https://badges.pufler.dev) [![GitHub stars](https://img.shields.io/github/stars/arrun99/arrunsuthahararajah.ca.svg)](https://github.com/arrun99/arrunsuthahararajah.ca/stargazers) [![GitHub forks](https://img.shields.io/github/forks/arrun99/arrunsuthahararajah.ca.svg)](https://github.com/arrun99/arrunsuthahararajah.ca/network)
