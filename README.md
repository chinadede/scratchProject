mkdir scratch
cd Scratch
git clone https://github.com/llk/scratch-gui # 如果你有修改，切换到你的副本
git clone https://github.com/llk/scratch-vm # 如果你有修改，切换到你的副本
git clone https://github.com/llk/scratch-blocks# 如果你有修改，切换到你的副本
cd scratch-vm
npm install
npm link
cd ../scratch-gui
npm install
npm link scratch-vm scratch-blocks  
npm install
npm start
http://localhost:8601/