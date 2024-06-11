
## Script to install

echo "Installing git..."
sudo apt-get update > /dev/null
sudo apt-get install -y git > /dev/null

echo "Cloning stable configuration"
git clone -b stable https://github.com/mattnics/MacBook_Ubuntu.git ~/.local/share/macbookconfig > /dev/null

source ~/.local/share/macbookconfig/install.sh
