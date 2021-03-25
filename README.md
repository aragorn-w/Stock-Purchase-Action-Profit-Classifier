# Stock-Purchase-Action-Profit-Classifier
Neural network to classify if buying or selling a tech stock would gain the most profit in a short period

CHANGE THE LENGTH OR VALUE OF THE CONFIG VARIABLES IN THE CODE TO SEE DIFFERENT RESULTS OR OUTPUT SHAPES
pred_delta_t = 15 --> how many days to predict into the future whether buying or selling would be most profitable

thresh_vec = {0.04: 'Fair', 0.10: 'Moderate', 0.16: 'Strong'} --> confidence levels for respectively buying and selling (ex. 5 outupt classes, Strong Buy | Decent Buy | Hold | Decent Sell | Strong Sell)

sml_period_lengths = [10, 25, 50] --> working day Small, Medium, and Long time periods to retrieve single-timeperiod technical indicators for each stock

start_date = int(datetime(2011, 12, 31).timestamp()) --> start date for historical data collection
end_date = int(datetime(2021, 3, 18).timestamp()) --> end date for historical data collection
