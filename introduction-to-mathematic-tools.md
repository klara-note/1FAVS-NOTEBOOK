<!-- Global site tag (gtag.js) - Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-1PSLTF4HCS"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-1PSLTF4HCS');
</script>
# 集合入門

意味論の中でも特に、形式的な道具を用いて意味的現象を説明しようとする理論を総じて形式意味論という。形式意味論の多くの手法で、数学、特に素朴な集合の概念が用いられている。このノートでは、最低限必要となる集合概念について素描する。

## 1. 基本的な概念

**集合**とは、何らかのものの集まりのことである。集合を書き表すとき、その要素を波括弧$\{,\}$で囲って表すことがある。

- 例

  $0$以上$10$以下の奇数の集合は$\{1,3,5,7,9\}$と表せる。

  英語のアルファベットのうち、はじめの5つの集合は$\{a,b,c,d,e\}$と表せる。

### 1.1 集合間の関係

ある集合$A$に$a$が含まれているとき、$a$を$A$の**元**、あるいは**要素**という。$a$が$A$の元であることは次のように表記される。
$$
a\in A
$$

- 例

  $1\in \{1,3,5,7,9\}$である。

二つの集合$A,B$について、$A$の元すべてが$B$に属するとき、$A$は$B$に含まれる、あるいは$A$は$B$の**部分集合**であるという。これは$A$が$B$にスッポリと包まれているような状態である。$A$が$B$の部分集合であることは次のように表記される。
\\[
A\subset B
\\]

- 例
	
	$\{1,5\}\subset \{1,3,5,7,9\}$である。

また、$A\subset B$と$B\subset A$が同時に成り立つとき、$A$は$B$に包まれていて、逆に$B$は$A$に包まれているということであり、つまり$A$と$B$は一致している。したがって$A\subset B$と$B\subset A$が同時に成り立つことを$A$と$B$は**等しい**という。$A$と$B$が**等しい**ことは次のように表記される。

\\[
A=B
\\]

また、要素を一つも持たない集合、つまり集合$\{\}$を空集合といい、$\empty$や$\varnothing$と書く。集合$A$どんな集合であっても$\varnothing \subset A$が成立する。

<details>
  <summary>さらに詳しく</summary>
  部分集合の定義より、$\varnothing\subset A$が成立することと、$a\in\varnothing$をみたす全ての$a$について$a\in A$が成立することは同値である。ところで、$\varnothing$は一切の要素を持たないから、「$a\in\varnothing$をみたす全ての$a$について$a\in A$」の前提は$a$が何であっても成立せず、論理的に「$a\in\varnothing$をみたす全ての$a$について$a\in A$」は常に成立する。(cf. 全称量化)
</details>

### 1.2 集合間の演算