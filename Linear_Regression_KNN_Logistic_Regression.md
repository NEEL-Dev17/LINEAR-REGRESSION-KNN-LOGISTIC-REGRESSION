#REGRESSION SCORE 1
import pandas as pd
import numpy as np
from sklearn.model_selection import train_test_split
from sklearn.linear_model import LinearRegression
from sklearn.metrics import mean_absolute_error, mean_squared_error, r2_score
import matplotlib.pyplot as plt
data = pd.read_csv('student_sleep_patterns.csv')
X = data[['Age']]  
y = data['Screen_Time']  
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)
model = LinearRegression()
model.fit(X_train, y_train)
y_pred = model.predict(X_test)
mae = mean_absolute_error(y_test, y_pred)
mse = mean_squared_error(y_test, y_pred)
rmse = np.sqrt(mse)
r2 = r2_score(y_test, y_pred)
mape = np.mean(np.abs((y_test - y_pred) / y_test)) * 100
print("Mean Absolute Error (MAE):",mae)
print("Mean Squared Error (MSE):", mse)
print("Root Mean Squared Error (RMSE):",rmse)
print("R-squared (R2):",r2)
print("Mean Absolute Percentage Error (MAPE):",mape,"%")
plt.scatter(X, y, color='blue', label='Actual Data')  
plt.plot(X, model.predict(X), color='red', label='Regression Line')  
plt.title("Age vs Screen Time")
plt.xlabel("Age")
plt.ylabel("Screen Time")
plt.legend()
plt.grid()
plt.show()

#REGRESSION SCORE 2
import pandas as pd
import numpy as np
from sklearn.model_selection import train_test_split
from sklearn.linear_model import LinearRegression
from sklearn.metrics import mean_absolute_error, mean_squared_error, r2_score
import matplotlib.pyplot as plt
data = pd.read_csv('student_sleep_patterns.csv')
X = data[['Age']]  
y = data['Sleep_Duration']  
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)
model = LinearRegression()
model.fit(X_train, y_train)
y_pred = model.predict(X_test)
mae = mean_absolute_error(y_test, y_pred)
mse = mean_squared_error(y_test, y_pred)
rmse = np.sqrt(mse)
r2 = r2_score(y_test, y_pred)
mape = np.mean(np.abs((y_test - y_pred) / y_test)) * 100
print("Mean Absolute Error (MAE):",mae)
print("Mean Squared Error (MSE):", mse)
print("Root Mean Squared Error (RMSE):",rmse)
print("R-squared (R2):",r2)
print("Mean Absolute Percentage Error (MAPE):",mape,"%")
plt.scatter(X, y, color='blue', label='Actual Data')  
plt.plot(X, model.predict(X), color='red', label='Regression Line')  
plt.title("Age vs Sleep_Durration")
plt.xlabel("Age")
plt.ylabel("Sleep_Durration")
plt.legend()
plt.grid()
plt.show()

#REGRESSION SCORE 3
import pandas as pd
import numpy as np
from sklearn.model_selection import train_test_split
from sklearn.linear_model import LinearRegression
from sklearn.metrics import mean_absolute_error, mean_squared_error, r2_score
import matplotlib.pyplot as plt
data = pd.read_csv('student_sleep_patterns.csv')
X = data[['Age']]  
y = data['Caffeine_Intake']  
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)
model = LinearRegression()
model.fit(X_train, y_train)
y_pred = model.predict(X_test)
mae = mean_absolute_error(y_test, y_pred)
mse = mean_squared_error(y_test, y_pred)
rmse = np.sqrt(mse)
r2 = r2_score(y_test, y_pred)
mape = np.mean(np.abs((y_test - y_pred) / y_test)) * 100
print("Mean Absolute Error (MAE):",mae)
print("Mean Squared Error (MSE):", mse)
print("Root Mean Squared Error (RMSE):",rmse)
print("R-squared (R2):",r2)
print("Mean Absolute Percentage Error (MAPE):",mape,"%")
plt.scatter(X, y, color='blue', label='Actual Data')  
plt.plot(X, model.predict(X), color='red', label='Regression Line')  
plt.title("Age vs Caffeine_Intake")
plt.xlabel("Age")
plt.ylabel("Caffeine_Intake")
plt.legend()
plt.grid()
plt.show()

#REGRESSION SCORE 4
import pandas as pd
import numpy as np
from sklearn.model_selection import train_test_split
from sklearn.linear_model import LinearRegression
from sklearn.metrics import mean_absolute_error, mean_squared_error, r2_score
import matplotlib.pyplot as plt
data = pd.read_csv('student_sleep_patterns.csv')
X = data[['Age']]  
y = data[' Study_Hours']  
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)
model = LinearRegression()
model.fit(X_train, y_train)
y_pred = model.predict(X_test)
mae = mean_absolute_error(y_test, y_pred)
mse = mean_squared_error(y_test, y_pred)
rmse = np.sqrt(mse)
r2 = r2_score(y_test, y_pred)
mape = np.mean(np.abs((y_test - y_pred) / y_test)) * 100
print("Mean Absolute Error (MAE):",mae)
print("Mean Squared Error (MSE):", mse)
print("Root Mean Squared Error (RMSE):",rmse)
print("R-squared (R2):",r2)
print("Mean Absolute Percentage Error (MAPE):",mape,"%")
plt.scatter(X, y, color='blue', label='Actual Data')  
plt.plot(X, model.predict(X), color='red', label='Regression Line')  
plt.title("Age vs Study_Hours")
plt.xlabel("Age")
plt.ylabel("Study_Hours")
plt.legend()
plt.grid()
plt.show()

#REGRESSION 5
import pandas as pd
import numpy as np
from sklearn.model_selection import train_test_split
from sklearn.linear_model import LinearRegression
from sklearn.metrics import mean_absolute_error, mean_squared_error, r2_score
import matplotlib.pyplot as plt
data = pd.read_csv('student_sleep_patterns.csv')
X = data[['Age']]  
y = data[' Physical_Activity']  
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)
model = LinearRegression()
model.fit(X_train, y_train)
y_pred = model.predict(X_test)
mae = mean_absolute_error(y_test, y_pred)
mse = mean_squared_error(y_test, y_pred)
rmse = np.sqrt(mse)
r2 = r2_score(y_test, y_pred)
mape = np.mean(np.abs((y_test - y_pred) / y_test)) * 100
print("Mean Absolute Error (MAE):",mae)
print("Mean Squared Error (MSE):", mse)
print("Root Mean Squared Error (RMSE):",rmse)
print("R-squared (R2):",r2)
print("Mean Absolute Percentage Error (MAPE):",mape,"%")
plt.scatter(X, y, color='blue', label='Actual Data')  
plt.plot(X, model.predict(X), color='red', label='Regression Line')  
plt.title("Age vs Physical_Activity")
plt.xlabel("Age")
plt.ylabel("Physical_Activity")
plt.legend()
plt.grid()
plt.show()

#KNN ANALYSIS
from sklearn.model_selection import train_test_split
from sklearn.neighbors import KNeighborsRegressor
from sklearn.preprocessing import StandardScaler
from sklearn.metrics import mean_squared_error, r2_score
import numpy as np
import matplotlib.pyplot as plt
X = data[['Age']].values  # Feature: Age
y = data['Sleep_Duration'].values  # Target: Sleep Duration
scaler = StandardScaler()
X_scaled = scaler.fit_transform(X)
X_train, X_test, y_train, y_test = train_test_split(X_scaled, y, test_size=0.33, random_state=42)
k = 5  
knn = KNeighborsRegressor(n_neighbors=k)
knn.fit(X_train, y_train)
y_pred = knn.predict(X_test)
mse = mean_squared_error(y_test, y_pred)
r2 = r2_score(y_test, y_pred)
print("Mean Squared Error (MSE):", mse)
print("R-squared (R²):", r2)
plt.figure(figsize=(8, 6))
plt.scatter(X_test, y_test, color='blue', label='Actual Data', alpha=0.6)
plt.scatter(X_test, y_pred, color='red', label='Predicted Data', alpha=0.6)
plt.title(f'k-NN Regression (k={k})')
plt.xlabel('Age (Normalized)')
plt.ylabel('Sleep Duration')
plt.legend()
plt.grid(alpha=0.3)
plt.show()

#LOGISTIC REGRESSION
from sklearn.model_selection import train_test_split
from sklearn.linear_model import LogisticRegression
from sklearn.preprocessing import StandardScaler
from sklearn.metrics import accuracy_score, classification_report
import numpy as np
import pandas as pd
threshold = data['Screen_Time'].median()  
data['Screen_Time_Class'] = np.where(data['Screen_Time'] > threshold, 1, 0)  
X = data[['Age']].values  # Age as the feature
y = data['Screen_Time_Class'].values  # Categorical Screen_Time (High=1, Low=0)
scaler = StandardScaler()
X_scaled = scaler.fit_transform(X)
X_train, X_test, y_train, y_test = train_test_split(X_scaled, y, test_size=0.33, random_state=42)
log_reg = LogisticRegression()
log_reg.fit(X_train, y_train)
y_pred = log_reg.predict(X_test)
accuracy = accuracy_score(y_test, y_pred)
print("Accuracy:", accuracy)
print("Classification Report:\n", classification_report(y_test, y_pred))
import matplotlib.pyplot as plt
plt.figure(figsize=(8, 6))
plt.scatter(X_test, y_test, color='blue', label='Actual Data', alpha=0.6)
plt.scatter(X_test, y_pred, color='red', label='Predicted Data', alpha=0.6)
plt.title('Logistic Regression: Age vs. Screen Time (High vs. Low)')
plt.xlabel('Age (Normalized)')
plt.ylabel('Screen Time Classification')
plt.legend()
plt.grid(alpha=0.3)
plt.show()
