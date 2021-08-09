# PriceDif


Although extensive and detailed market data are constantly publicized by the market operator, historical market data are not utilized effectively to reduce the imbalance cost. This study initially casts the imbalance cost reducing problem as a binary classification problem and constructs a framework that consists of a long short term memory autoencoder and a blend of advanced classifiers. Then, the method extracts information from the market data if the day-ahead or imbalance price will be higher at a given hour of the next day. Using this information, auxiliary algorithms alter existing production forecasts and prevents abrupt rises in the imbalance cost.

A recent study published in Applied Energy proposes an approach to anticipate the imbalance cost spikes through mining in the market data and then it avoids them by amending existing wind power forecasts. Previous studies related to the imbalance cost have mostly focused on market design for a broader integration of renewables, assessment and mitigation of imbalance risks in the grid, uncertainty analysis of market conditions and risk management for day-ahead and intraday market bidding strategies. A small number of studies have considered the subject from a generator’s perspective and relatively fewer methods have been proposed to reduce the imbalance cost of a wind generator directly in real market conditions. To our best knowledge, a way of effectively utilizing the market data to reduce the imbalance cost has not been developed before, although this cost is determined in marketplace and the market operators are regularly publishing extensive data.

The study aims to reduce the annual imbalance cost of a wind producer using the information extracted from the market data without any assumption on market prices. The proposed method is designed to be employed six hours before the day-ahead market closure time.

The main contributions and novelty of this paper are

The study describes a way of utilizing market data in order to amend the pre-generated wind power forecasts for reducing the imbalance cost of a generator.
It defines the imbalance cost reducing problem as a binary classification problem to mine in the market data.
It develops a complete framework that is composed of a long short term memory recurrent neural network and a blend of classifiers along with the algorithms for autonomously amending the forecasts.
The proposed framework can be adapted to any wind power forecasting system and it does not require predictions of the day-ahead and balancing market prices.
The method works reliably and it is robust to sudden changes (i.e. ramps) in power production and in market prices. 
The method particularly avoids outrageous imbalances which occur in the instances when the difference between marginal and day-ahead prices is high and the prediction accuracy is low. An algorithm is developed to alter the wind power forecasts adaptively.
The proposed method initially preprocess the data using a long short term memory (LSTM) autoencoder and then it combines five binary classifiers to construct a hybrid classifier. The results show that the LSTM autoencoder improves the accuracy all classifiers and the hybrid classifier gives the best accuracy of 61.08%. The method therefore extracts information whether the day-ahead or balancing market price will be higher at a given hour of the next day. Then, using this information, auxiliary algorithms alter existing production forecasts and prevents abrupt rises in the imbalance cost. The tests show that the proposed method consistently reduces the imbalance cost. The method is robust to varying number of sudden changes (i.e. ramps) in both wind power production and the marginal price. As the accuracy of the hybrid classifier increases, reduction in the balancing cost tends to increase.

The proposed method has resulted in 6.2581%, 8.2402%, 11.195% and 9.9037% reduction for wind power plants (WPPs) 1-4, respectively. The proposed method works reliably well and in 96% of the tested months, the method has reduced the cost. The proposed method is adaptable to any forecasting system and it is concluded that the method has capability of reducing the balancing cost of a wind generator more than 10%.

** The content has been copied from "Dinler, A., Reducing balancing cost of a wind power plant by deep learning in market data: A case study for Turkey" Applied Energy (2021). See the article for details. https://doi.org/10.1016/j.apenergy.2021.116728
