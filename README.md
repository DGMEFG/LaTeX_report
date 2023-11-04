# LaTeX_report

🟥 简单三线表：

<img src=".\md_pic\p1.png" style="zoom:40%;" />

code : 

```tex
\begin{table}[htbp]
	\centering
	\caption{符号说明}
	\begin{tabularx}{0.9\textwidth}{@{}cl@{}}
		\toprule
		符号 & 说明 \\
		\midrule
		$\mathcal{F}$ & 使用非线性函数$\mathcal{F}$表示神经网络 \\
		$(\mathrm{x}^i,y^i)$ & 第 $i$ 张训练图片，及其对应的标签 $y_i$ \\
		$o^i = \mathcal{F}(\mathrm{x}^i)$ & 神经网络输出的logits \\
		$C$ & 本任务分类的总类别的数目\\
		$\tilde{p}^i = \mathrm{softmax(o^i)}$ & 用以表示使用softmax激活后的值\\
		$N$&一个小批次的样本数目\\
		$N_c$&在一个小批次中，真实标签为 $c$ 的训练样本的数目\\
		\bottomrule
	\end{tabularx}
\end{table}
```



🟥 插入图片：

<img src=".\md_pic\p2.png" style="zoom:60%;" />

code:

```tex
\begin{figure}[htbp]
	\centering
	\includegraphics[scale=0.56]{./pic/block.png}
	\caption{残差块}
\end{figure}
```



 🟥 普通代码块

之前看到一个很漂亮的代码块，之后去更新一下

<img src=".\md_pic\p3.png" style="zoom:48%;" />

code: 

```tex
\begin{lstlisting}
conda create -n ML python==3.10
conda activate ML
\end{lstlisting}
```



🟥 结果展示表格

<img src = ".\md_pic\p4.png" style="zoom:50%">

code:

```tex
\begin{table}[htbp]
	\centering
	\begin{tabularx}{0.8\textwidth}{p{1cm}p{1cm}ccc}
		\toprule
		$t_{\mathrm{new}}$ & $t_{\mathrm{old}}$ & \heiti{Geometric Mean} & \heiti{Harmonic Mean} &\heiti{ Lowest Recall} \\
		\midrule
		1 & 1 & 40.5 & 33.6 & 4.0\\
		1 & 2 & 40.6 & \textbf{34.3} & \textbf{5.0}\\
		1 & 3 & 40.2 & 33.2 & 4.0\\
		\midrule
		2 & 1 & 39.0 & 31.0 & 3.0\\
		2 & 2 & \textbf{40.6} & 33.6 & 4.0\\
		\midrule
		3 & 1 & 31.2 & 21.4 & 2.0\\
		3 & 2 & 40.1 & 32.0 & 3.0\\
		\bottomrule
	\end{tabularx}
	\caption{$t_1,t_2$在 MISLAS+GML 模型上对ensemble的影响}
	\label{tab:table}
\end{table}
```

🟥 参考文献

```tex
\begin{thebibliography}
		\bibitem{1} Zhang, Yifan and Kang, Bingyi and Hooi, Bryan and Yan, Shuicheng and Feng, Jiashi, Deep 		long-tailed learning: A survey, arXiv preprint arXiv:2110.04596, 2021.
\end{thebibliography}
```





