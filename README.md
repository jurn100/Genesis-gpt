# Genesis-gpt
A character-level GPT trained on the Book of Genesis (KJV)

This project trains a character-level GPT model on the Book of Genesis (King James Version).  
The model generates new passages in the archaic, poetic style of the text.

Set up Instructions - how to run the project on their computer:
Clone the repository:
   ```bash
   git clone https://github.com/jurn100/genesis-gpt.git
   cd genesis-gpt

Create a virtual environment:
python -m venv venv
source venv/bin/activate  # (Mac/Linux)
venv\Scripts\activate     # (Windows)

Then Install Dependencies
pip install -r requirements.txt


How to Train the Model  

To train the model on Genesis, run:
```bash
python train.py train --input input.txt --save genesis_model.pth --steps 5000 --context-size 256 --batch-size 64 --n-embd 384 --n-head 6 --n-layer 6 --dropout 0.2 --lr 3e-4



How to Generate Text

To generate text with no prompt:
```bash
python train.py eval --load genesis_model.pth --token-count 500




