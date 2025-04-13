# mental-health

The original notebook is available on Kaggle (https://www.kaggle.com/code/adilshamim8/student-depression).
We implemented it with some minor modifications. The important point to note is that the software implementation (https://www.ellisonacademy.com/portfolio/students-depression) cannot be done directly as in the Kaggle notebook. It requires Numpy version compatibility and, in addition, downloading both the model and the scaler object, without which the result cannot be the same.

We attach the relevant code sections.

### Download scaler with Pickle
import pickle

### Save scaler to file
with open('students_scaler.pkl', 'wb') as f:
    pickle.dump(scaler, f)

from google.colab import files

### This will download scaler.pkl to your local machine
files.download('students_scaler.pkl')
