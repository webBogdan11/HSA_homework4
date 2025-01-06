# Load Testing Results

## Test Configuration

I executed my `siege-urls.txt` files with 4 different concurrency levels:

1.  siege -c 25 -t 30S -v -H 'Content-Type: application/json' -f siege-urls.txt
2.  siege -c 50 -t 30S -v -H 'Content-Type: application/json' -f siege-urls.txt
3.  siege -c 75 -t 30S -v -H 'Content-Type: application/json' -f siege-urls.txt
4.  siege -c 100 -t 30S -v -H 'Content-Type: application/json' -f siege-urls.txt

## Tested Endpoints

The `siege-urls.txt` file contains 2 endpoints:

1. `POST /items`
2. `GET /items`

## Results

### 25 Concurrent Users
![results for 25 concurrencies](./images/results-25.jpeg)

### 50 Concurrent Users
![results for 50 concurrencies](./images/results-50.jpeg)

### 75 Concurrent Users
![results for 75 concurrencies](./images/results-75.jpeg)

### 100 Concurrent Users
![results for 100 concurrencies](./images/results-100.jpeg)