# Scintill-AI
A research project aiming to apply machine learning models for regional Global Navigation Satellite System (**GNSS**) **ionospheric scintillation forecasting** at low latitudes.

## Table of Contents

- [What is it?](#what-is-it)

- [How can I run it?](#how-can-i-run-it)

    - [Spin up a container 🐋](#spin-up-a-container-)

    - [Connect to the cloud ☁️](#connect-to-the-cloud-)

## What is it?

The ionosphere contains ionised particles that are generally homogeneously distributed, and GNSS receivers – which use the signals from satellites orbiting the Earth to calculate their locations – can account for their effect on satellite signals using models. However, problems arise when there are irregularities, *i.e.* **localised fluctuations in the electron density** of the ionosphere, which can distort the phase and amplitude of GNSS signals, producing fluctuations known as *scintillations*.

The appearance of scintillation is often deemed unpredictable. It varies throughout the day, with sunset triggering a sharp increase in ionospheric activity that can last several hours. Also, an increase in solar activity can produce scintillation events that can **degrade the quality of satellite signals**. In standard GNSS receivers, a mild scintillation can degrade position accuracy by up to several metres. More severe scintillation can cause cycle slips or, in the most extreme cases, total loss of signal lock. So, whether it comes to precision agriculture in Brazil, oil exploration in Alaska or a large construction project in Singapore, it is highly beneficial to forecast the onset of scintillation.

👉 **For full details on the models and data, please refer to the repo of the [parent project](https://github.com/viventriglia/scintill-ai)**

## How can I run it?

### Spin up a container 🐋

- Clone the repo and ensure that the Docker daemon is running

- Build a Docker image: `docker build -t scintill-ai-web-app .`

- Run a container and expose it on a preferred port (for example, 8080): `docker run --rm -p 8080:5000 scintill-ai-web-app`

### Connect to the cloud ☁️

⚠️ The web app may be slower 🐌

- Access the [cloud instance](https://scintill-ai-web-app.onrender.com/)