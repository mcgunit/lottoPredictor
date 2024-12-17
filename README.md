
# Sequence Predictor

## To check

    - Small-to-Medium Data:
        Use TCNs or hybrid models (CNN + LSTM).
    - Large Data:
        Transformers are ideal due to scalability and performance.
    - If Sequence Dependencies are Weak:
        Pure CNN models like ResNet, EfficientNet, or MobileNet (better than GoogLeNet for general tasks).

## Installation

To install, you will need to have Python 3.x and the following libraries installed:
- numpy
- tensorflow
- keras
- art
- keras-tcn

You can install these libraries using pip by running the following command:

Using the requirements file:

```
    python3 -m pip install -r requirements.txt
```

For CPU only: 
```
    python3 -m pip install numpy tensorflow keras art pandas scikit-learn matplotlib keras-tcn
```

For GPU enabled:

```
    python3 -m pip install numpy tensorflow[and-cuda] keras art pandas scikit-learn matplotlib keras-tcn
```

## How to run

To run the complete flow run:

```
    python3 Predictor.py
```

To test model specific for example LSTM run:

```
    python3 LSTM.py
```

Check the __main__ section of the LSTM.py or GRU.py for pointing to data and set parameters for testing.

## Testing

To test a model when modifying or tuning you can run the LSTM.py or GRU.py directly and check the __main__ section. Use the test folder for trainingData and models if you don't want to touch the actual data (highly recommended). 

For testing You, in the `test` folder, can manually remove the last result from the .csv files and put it in the `sequenceToPredict_xxx.json` file. Then when tuning or changing the model, the results are compared. **It is of importance to take the latest result out of the test data**.


## Disclaimer

The code within this repository comes with no guarantee, the use of this code is your responsibility. I take NO responsibility and/or liability for how you choose to use any of the source code available here. By using any of the files available in this repository, you understand that you are AGREEING TO USE AT YOUR OWN RISK. Once again, ALL files available here are for EDUCATION and/or RESEARCH purposes ONLY.
Please keep in mind that while LSTM.py uses advanced machine learning techniques to predict lottery numbers, there is no guarantee that its predictions will be accurate. Lottery results are inherently random and unpredictable, so it is important to use LSTM responsibly and not rely solely on its predictions.

## License

This project is licensed under the [MIT License](https://opensource.org/licenses/MIT). You are free to use, modify, and distribute this project as long as you give attribution to the original author.
