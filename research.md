# Research – Xerox Queue Predictor

## 1. Problem Statement

I noticed that students visiting the photocopy shop at NIT Jamshedpur sometimes have to wait without knowing how long their work will take.

- The shop handles photocopies, B&W prints and colour prints.
- Different jobs take different amounts of time depending on the number of pages and type of service.
- Students often have to ask the shopkeeper for an estimated waiting time.
- I decided to build a small tool that estimates printing time and queue waiting time using actual job records.

## 2. Existing Solutions

### 1. Manual Queue Management

Small shops generally manage orders manually and estimate completion time based on experience. This can work for a small number of customers, but estimating waiting time becomes difficult when several jobs are pending.

### 2. QRPress

Website: https://www.qrpress.in/print-shop-software

QRPress provides digital print order and queue management features. However, I want to build something simpler that focuses mainly on predicting waiting time using the shop's own printing records, without requiring a complete order management system.

## 3. Sources Read

### Source 1: University Printing Shop – Waiting Time Research (2019)

Link: https://doi.org/10.37134/jsml.vol7.4.2019

- This paper discusses customer waiting time in a university printing shop.
- It uses actual observations and staff interviews to study the queue.
- It helped me understand why recording job timings is important for estimating waiting time.

### Source 2: QRPress – Print Shop Software

Link: https://www.qrpress.in/print-shop-software

- I explored this software to understand how existing print shops manage orders.
- It provides features for digital orders and print queue management.
- I used it as a reference while deciding to build a smaller tool focused on waiting-time prediction.

## 4. Initial Approach

I plan to use Python and Streamlit to build this tool. It will read printing records from a CSV file, calculate the average time per page for each service and estimate how long a new job or existing queue might take.

The estimates will be approximate because factors like printer issues, paper jams and workload can affect actual completion time.

## 5. Field Details

- **Place:** NIT Jamshedpur photocopy shop
- **Person interviewed:** Nitesh
- **Role:** Shopkeeper
- **Date:** 17/11/27
