## Week 2 Quiz

---

#### 1. What is a windowed dataset?

- [ ] A consistent set of subsets of a time series
- [ ] The time series aligned to a fixed shape
- [ ] There’s no such thing
- [x] `A fixed-size subset of a time series`

#### 2. What does ‘drop_remainder=true’ do?

- [x] `It ensures that all rows in the data window are the same length by cropping data` 
- [ ] It ensures that the data is all the same shape
- [ ] It ensures that all rows in the data window are the same length by adding data 
- [ ] It ensures that all data is used

#### 3. What’s the correct line of code to split an n column window into n-1 columns for features and 1 column for a label

- [ ] dataset = dataset.map(lambda window: (window[n-1], window[1]))
- [x] `dataset = dataset.map(lambda window: (window[:-1], window[-1:]))`
- [ ] dataset = dataset.map(lambda window: (window[-1:], window[:-1]))
- [ ] dataset = dataset.map(lambda window: (window[n], window[1]))

#### 4. What does MSE stand for?

- [ ] Mean Series error
- [ ] Mean Slight error
- [x] `Mean Squared error` 
- [ ] Mean Second error

#### 5. What does MAE stand for?

- [ ] Mean Average Error
- [ ] Mean Advanced Error
- [x] `Mean Absolute error` 
- [ ] Mean Active Error

#### 6. If time values are in time[], series values are in series[] and we want to split the series into training and validation at time 1000, what is the correct code?

- [ ] time_train = time[split_time]

      x_train = series[split_time]
      time_valid = time[split_time]
      x_valid = series[split_time]
      
- [ ] Mean Advanced Error
- [x] `Mean Absolute error` 
- [ ] Mean Active Error
