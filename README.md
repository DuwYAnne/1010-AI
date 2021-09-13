# 1010-AI

This project attempts to use deep learning to play the game [1010!](https://play.google.com/store/apps/details?id=com.gramgames.tenten&hl=en_US&gl=US), a game similar to tetris on a 10x10 board where you are given bags of 3 shapes at a time, and you have to fill the board as much as possible, and a filled column/row gets completely cleared.

The AI was never very strong due to possibly a few issues. One is that the output layer is quite large, and the AI was unable to train all the variables with limited computational power. Another is that invalid moves can still be played, just with a negative reward, so the AI will play invalid moves, often resulting in a score of 0. Another issue that prevents good play could be that although the input layer is passed with one-hot encoding, the output layer was too small to correctly be able to utilize all the information, and it was difficult to increase the size as my device was too computationally weak. 

Regardless of all this, the AI was still able to improve from an average score of **1** through random moves, to an average score of **7** after 5000 episodes. The maximum score it achieved was 14.

![Graph](https://i.imgur.com/ETCZaNK.png)

## References

Inspired by: https://pytorch.org/tutorials/intermediate/reinforcement_q_learning.html
