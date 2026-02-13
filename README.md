# Ride Cancellation Analysis 

## Problem Statement

A ride-hailing platform experiences order failures when customers don't successfully get a car. This project analyzes failed orders to identify key failure patterns—including cancellations
(before/after driver assignment) and rejections—and investigates how these failures vary by time of day. By examining metrics like cancellation timing and estimated time of arrival (ETA),
this project aims to uncover operational insights that could improve match success rates and customer experience.

## Tech Stack
 Language: Python
 Libraires: Numpy, Pandas, Matplotlib
 Visualization: Excel

## Data Description
We have two data sets: data_orders and data_offers, both being stored in a CSV format. The data_orders data set contains the following columns:

order_datetime - time of the order
origin_longitude - longitude of the order
origin_latitude - latitude of the order
m_order_eta - time before order arrival
order_gk - order number
order_status_key - status, an enumeration consisting of the following mapping:
4 - cancelled by client,
9 - cancelled by system, i.e., a reject
is_driver_assigned_key - whether a driver has been assigned
cancellation_time_in_seconds - how many seconds passed before cancellation
The data_offers data set is a simple map with 2 columns:

order_gk - order number, associated with the same column from the orders data set
offer_id - ID of an offer
