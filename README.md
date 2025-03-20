# Flow 3 Auto Bot

This is an automated tool for managing Flow 3 accounts, handling referrals, completing daily tasks, and running a bot farm for automatic mining. This bot helps automate processes for Flow 3 extension users.

## Features

- **Auto Referral**: Create new accounts using referral codes
- **Auto Task and Daily**: Complete daily tasks and regular tasks for existing accounts
- **Run Bot Farm**: Continuously run mining operations with automatic pinging

## Requirements

- Python 3.8 or higher
- Required Python packages (install via `pip install -r requirements.txt`):

## Setup Instructions

1. Clone the repository:
```
git clone https://github.com/kelliark/Flow3-AutoBot
cd Flow3-AutoBot
```
2. Install the required packages:
```
pip install -r requirements.txt
```
3. Prepare your configuration files:
- `codes.txt`: Your referral codes (for Auto Referral mode)
- `wallets.txt`: Your wallet details (for Auto Task and Daily / Bot Farm modes)
- Proxy files (optional but recommended):
  - `refproxies.txt`: Proxies for Auto Referral mode
  - `tdproxies.txt`: Proxies for Auto Task and Daily mode
  - `farmproxies.txt`: Private proxies for Bot Farm mode

## Configuration Files Format

### wallets.txt
```
Wallet: wallet_address_here | Private: private_key_here
```
### codes.txt
One referral code per line:
```
referral_code_1
referral_code_2
```
### Proxy files (refproxies.txt, autotd.proxies, farmproxies.txt)
One proxy per line:
```
ip:port
protocol://username:password@ip:port
username:password@ip:port
```

## Usage
Run the main script:
```
python main.py
```

Then follow the on-screen instructions to select your desired mode:

1. **Auto Referral**: Creates new accounts using the referral codes in codes.txt
2. **Auto Task and Daily**: Uses existing accounts to complete tasks and daily activities
3. **Run Bot Farm**: Runs the bot in farming mode for automatic mining
   - Has options for using Monosans proxies (auto-updated), private proxies, or no proxies

## Notes
- For best results, use proxies for each operation as some services may limit access from a single IP
- Running too many accounts from a single IP may lead to bans or restrictions
- This tool is for educational purposes only

## Disclaimer
This tool is provided for educational purposes only. Users are responsible
