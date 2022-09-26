# Stock Notes

This is a collection of Jupyter notebooks used for stock and stock market analysis and crawling. Numpy, Pandas, Seaborn, Matplotlib, and other libraries are used in the code.

# Crawler

**Investors**

<img width="740" alt="스크린샷 2022-09-26 오후 9 23 59" src="https://user-images.githubusercontent.com/44548828/192275479-589ab52d-6e1f-4bd1-9e8a-75be874c125f.png">

**News**

<img width="740" alt="스크린샷 2022-09-26 오후 9 09 21" src="https://user-images.githubusercontent.com/44548828/192272670-3650ece8-9f17-42fd-a385-16f789616912.png">


# Analysis

**Risk Measure**

<img width="500" alt="스크린샷 2022-09-26 오후 9 21 46" src="https://user-images.githubusercontent.com/44548828/192274846-1d846c14-61b1-4583-b285-95b02f6acb6a.png">

**Fundamental Trend**

```
subplot_fundamental(['pbr', 'per', 'roe', 'eps'])
```

<img width="740" alt="스크린샷 2022-09-26 오후 9 34 06" src="https://user-images.githubusercontent.com/44548828/192277343-64ab0e98-8ccf-4cc4-9b77-3d0387d88295.png">

# Visualization

**Market Capitalization Ranking Trend**
```
kospi_marketcap_ranking_df = get_ranking_df(previous_year, today, freq='1M', market='kospi', ranking_type='marketcap')
plot_bump(kospi_marketcap_ranking_df, 30, "Kospi Market Cap")
```
<img width="740" alt="cap" src="https://user-images.githubusercontent.com/44548828/192274299-d93d6a54-ea17-42e6-835e-7a082cac9f8b.png">

**Market capitalization trend by industry**

```
fig = plt.figure(figsize=(20, 12))
ax = plt.subplot(111)
pd.DataFrame(data).plot.bar(stacked=True, ax=ax, color=colors)
ax.legend(loc='center left',  bbox_to_anchor=(1, 0.5), fancybox=True, shadow=True)
plt.show()
```

<img width="740" alt="captrend" src="https://user-images.githubusercontent.com/44548828/192284053-1ef52f39-880d-4096-957a-2dfdeec4b536.png">

**News Word Cloud**
```
analyser = Analyser(df)
analyser.get_wordcloud('Text')
```
<img width="740" alt="cap" src="https://user-images.githubusercontent.com/44548828/192278285-18ba7ba6-962f-49bb-befe-5719c812fa3d.png">

