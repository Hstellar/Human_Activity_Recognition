# Human_Activity_Recognition
##  UCI HAR dataset
<li>The pre-processing steps included:</li>
<li>Pre-processing accelerometer and gyroscope using noise filters. Sensor Data is captured at
frequency of 50 Hz.<li>
<li>Splitting data into fixed windows of 2.56 seconds (128 data points) with 50% overlap.Splitting
of accelerometer data into gravitational (total) and body motion components.</li>
<li>A number of time and frequency features commonly used in the field of human activity
recognition were extracted from each window. The result was a 561 element vector of
features.</li>
<li>The dataset was split into train (70%) and test (30%) sets based on data for subjects, e.g. 21
subjects for train and nine for test.</li>
<li>Own dataset - Matlab android application</li>

## ConvLSTM approach ##
<li>CNN ->read subsequences of the main sequences in block->extract feature from each
block</li>
<li>LSTM->interpret the features extracted from each block.</li>
<li>Input:</li>
<li>Samples: n, for the number of windows in the dataset.</li>
<li>Time: 4, for the four subsequences that we split a window of 128 time steps into.</li>
<li>Rows: 1, for the one-dimensional shape of each subsequence.</li>
<li>Columns: 32, for the 32 time steps in an input subsequence.</li>
<li>Channels: 9, for the nine input variables.</li>

## Model Summary ##
![model summary](https://drive.google.com/file/d/1Q1vY8TWxB6igd80cx00RRErchAQz4-jP/view?usp=sharing "Title is optional")
