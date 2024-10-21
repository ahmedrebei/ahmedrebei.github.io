---
title: "FSNet: A hybrid model for seasonal forecasting"
collection: publications
category: manuscripts
permalink: /publications/FSNet
excerpt: 'This study presents the Fourier Split NET (FSNET), a hybrid load forecasting model that combines Fourier transform for deseasonalization with LSTM neural networks to enhance prediction accuracy, addressing the challenges of autocorrelation and seasonality in load data.'
date: 2023-07-10
venue: 'IEEE Transactions on Emerging Topics in Computational Intelligence'
paperurl: 'https://ieeexplore.ieee.org/iel7/7433297/7777658/10177276.pdf'
citation: 'Rebei et al., 2023. FSNet: A hybrid model for seasonal forecasting. <i>IEEE Transactions on Emerging Topics in Computational Intelligence.</i>'
---

Load forecasting with low prediction error is essential to keep minimizing costs in generating and supplying power. It has many applications in energy production, distribution, and infrastructure construction. Because of the high autocorrelation and strong seasonality in load data, it is difficult to build robust and generalizable forecasting models. To address the problem, we propose a hybrid model, the Fourier Split NET (FSNET). The proposed model consists of two phases. A deseasonalization phase where the model uses the Fourier transform to isolate the seasonal component from the data using the fast Fourier transform. The second phase consists of training a simple linear model to replicate the seasonal behavior of the data and training a group of LSTM neural networks on different clusters of the data. The model uses statistical features to build separate LSTM models for different groups of data. We experimented on open datasets and obtained higher accuracy results compared to other forecasting approaches using different accuracy metrics.