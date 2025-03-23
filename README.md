# powerloom-update23032025 for single node user
# Navigate to your snapshotter directory
cd powerloom-mainnet

# Pull latest changes
git fetch
git checkout main
git pull

# Stop existing node and cleanup
./diagnose.sh -y

# Deploy with new chain configuration
./build.sh
