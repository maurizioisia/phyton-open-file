import pandas as pd
df = pd.read_csv("https://raw.githubusercontent.com/pcm-dpc/COVID-19/master/dati-andamento-nazionale/dpc-covid19-ita-andamento-nazionale.csv")

import matplotlib.pyplot as plt

# definiamo le dimensioni della finestra in pollici ed il dpi

from matplotlib.pyplot import figure
figure(figsize=(18,10), dpi=80)

x = df['date']=pd.to_datetime(df['data'])
y = df['nuovi_positivi'].rolling(7).mean()

plt.fill_between(x,y,color ='green', where =(y<20000))
plt.plot(x,y)
