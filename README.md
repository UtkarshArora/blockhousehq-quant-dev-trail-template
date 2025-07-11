1) video link: https://drive.google.com/file/d/18ElCKwhV6femQoP60A0fGGM92_nmlZzN/view?usp=sharing

2) Commands to run Kafka(via Docker): 

sudo apt update
sudo apt install docker.io docker-compose -y
sudo docker-compose up -d (since docker-compose.yml was already there in the repo)
docker ps

3) Running producer and backtest:
    python backtest.py

4) Screenshots:
https://drive.google.com/drive/folders/1a_wyKTmwTabvfDxNVJLi3rZ-Hqlu0MdD?usp=sharing

5) output.json:
{
    "best_parameters": {
        "lambda_over": 0.2,
        "lambda_under": 0.2,
        "theta_queue": 0.1
    },
    "optimized": {
        "total_cash": 1113715.0,
        "avg_fill_px": 222.743
    },
    "baselines": {
        "best_ask": {
            "total_cash": 1114117.28,
            "avg_fill_px": 222.823456
        },
        "twap": {
            "total_cash": 173049.30800000002,
            "avg_fill_px": 223.00168556701033
        },
        "vwap": {
            "total_cash": 1114117.28,
            "avg_fill_px": 222.823456
        }
    },
    "savings_vs_baselines_bps": {
        "best_ask": 3.6107509256116233,
        "twap": 11.600161960775798,
        "vwap": 3.6107509256116233
    }
}