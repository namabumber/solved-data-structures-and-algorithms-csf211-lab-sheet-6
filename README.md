Download Link: https://assignmentchef.com/product/solved-data-structures-and-algorithms-csf211-lab-sheet-6
<br>
<ol>

 <li>Given an array <strong><em>P </em></strong>with elements<strong><em> p<sub>1</sub>, p<sub>2</sub>, …, p<sub>n</sub></em></strong> and an <strong><em>n×n</em></strong> sized binary symmetric matrix <strong><em>A</em></strong>, you have to find the lexicographically minimum permutation which can be achieved by swapping two distinct elements <strong><em>p<sub>i</sub></em></strong> and <strong><em>p<sub>j</sub></em></strong> where the condition <strong><em>A[i][j]= 1</em></strong> holds and <strong><em>1 ≤ i, j ≤ n</em></strong>.</li>

</ol>




<strong>Input: </strong>

First line contains <strong><em>n</em></strong>.

Second line contains <strong><em>n</em></strong> elements of array <strong><em>P</em></strong>.

Each of the next <strong><em>n</em></strong> lines contains <strong><em>n<sup>2</sup></em></strong> integers which denote matrix <strong><em>A</em></strong> as a whole. <strong><em>A[i][j]</em></strong> <strong><em>= 1</em></strong> means <strong><em>p<sub>i</sub></em></strong> and <strong><em>p<sub>j</sub></em></strong> can be swapped, otherwise no swapping can be done.




<strong>Output: </strong>

The lexicographically minimum permutation that can be achieved by swapping.




<strong>Example: </strong>

<strong>Input: </strong>

7

5 2 4 3 6 7 1

0001001

0000000

0000010

1000001

0000000

0010000

1001000




<strong>Output</strong>:

1 2 4 3 6 7 5




<ol start="2">

 <li>You want to sort <strong><em>n</em></strong> different arrays (each of size <strong><em>m</em></strong>) simultaneously. You can choose a pair of distinct indices <strong><em>i</em></strong> and <strong><em>j</em></strong> (<strong><em>1 ≤ i</em></strong>, <strong><em>j ≤ m</em></strong>, <strong><em>i ≠ j</em></strong>). Then, in each array, the values at positions <strong><em>i</em></strong> and <strong><em>j</em></strong> are swapped only if the value at position <strong><em>i</em></strong> is strictly greater than the value at position <strong><em>j</em></strong>. You want to find an array containing pairs of distinct indices that, chosen in order, will sort all of the <strong><em>n</em></strong> arrays in ascending order or descending order.</li>

</ol>




<strong>Input: </strong>

Two integers <strong><em>n</em></strong> (no. of arrays) and <strong><em>m</em></strong> (size of each array) and <strong><em>k</em></strong> (<strong><em>k</em></strong> is zero if sorting is to be done in ascending order and 1 if sorting is to be done in descending order). Each of the next <strong><em>m</em></strong> lines contains the arrays of size <strong><em>m</em></strong>.




<strong>Output:  </strong>

In the first line of the output, print an integer <strong><em>p</em></strong>, the size of the array (<strong><em>p</em></strong> can be at most <strong><em>m*(m-1)/2</em></strong>). Each of the next <strong><em>p</em></strong> lines must contain two distinct integers <strong><em>i</em></strong> and <strong><em>j</em></strong> (<strong><em>1 ≤ i, j ≤ m, i ≠ j</em></strong>), representing the chosen indices.




<strong>Example: Input: </strong>

2 5 0

1 3 2 5 4

<ul>

 <li>4 3 2 5</li>

</ul>

<strong>Output: </strong>

3

<ul>

 <li>4</li>

</ul>

2 3

4 5




<ol start="3">

 <li>You are a dog lover and thus you don’t like cats. You live by an unusual park. The park is a rooted tree of <strong><em>n</em></strong> vertices with root node as 1. Vertex 1 also contains your house. Unfortunately, some vertices also contain cats and you know those vertices. You want to travel to each of the leaves of the tree starting from your house. But since you don’t like cats, if you encounter <strong><em>m</em></strong> consecutive cats in your path from your house to a leaf node then you drop the path.</li>

</ol>




<strong>Input:  </strong>

The first line contains two integers, <strong><em>n</em></strong> and <strong><em>m</em></strong> — the number of vertices of the tree and the maximum number of consecutive vertices with cats that is still ok for you.

The second line contains <strong><em>n</em></strong> integers <strong><em>a<sub>1</sub>, a<sub>2</sub>, …, a<sub>n</sub></em></strong> where each <strong><em>a<sub>i</sub></em></strong> either equals to 0 (then vertex <strong><em>i</em></strong> has no cat), or equals to 1 (then vertex <strong><em>i</em></strong> has a cat).

Each of the next <strong><em>n-1</em></strong> lines contains the edges of the tree in the format <strong><em>x<sub>i</sub></em></strong>, <strong><em>y<sub>i</sub></em></strong>, where <strong><em>x<sub>i</sub></em></strong> and <strong><em>y<sub>i</sub></em></strong> are the vertices of the tree, connected by an edge.




<strong>Output:  </strong>

A single integer — the number of distinct leaves of a tree, the path to which from your home contains at most <strong><em>m</em></strong> consecutive vertices with cats.




<strong>Example: </strong>

<strong>Input: </strong>

4 1

1 1 0 0

<h1><a name="_Toc10922"></a>1 2</h1>

<h1><a name="_Toc10923"></a>1 3</h1>

1 4

<strong>Output: </strong>

<h1><a name="_Toc10924"></a>2</h1>




<ol start="4">

 <li>You have <strong><em>n</em></strong> different socks with you. Each of the socks is of a colour. The total colours are <strong><em>k</em></strong>. Your mom is going out for a vacation and has made you a schedule for the <strong><em>m</em></strong> days she is going out for. For each of the <strong><em>m</em></strong> days, she has written down <strong><em>l[i], r[i]</em></strong> (<strong><em>l[i]</em></strong> denoting the left sock and <strong><em>r[i]</em></strong> denoting the right sock) which you will wear for the day. Now she was in a hurry and didn’t realise that you can’t wear socks of different colours on the same day. However, you possess <strong><em>k</em></strong> jars of paint – one for each colour. You want to fix the situation by swapping socks between the given pairs or/and recolouring some of them. Note that you want to change the colours of minimum number of socks.</li>

</ol>




<strong>Input:  </strong>

The first line of input contains three integers <strong><em>n, m</em></strong> and <strong><em>k</em></strong>— the number of socks, the number of days and the number of available colours respectively.

The second line contain <strong><em>n</em></strong> integers <strong><em>c<sub>1</sub>, c<sub>2</sub>, …, c<sub>n</sub> (1 ≤ c<sub>i</sub> ≤ k)</em></strong> — current colours of your socks.

The third line contains the number of socks for each colour.

Each of the following <strong><em>m</em></strong> lines contains two integers <strong><em>l<sub>i</sub></em></strong> and <strong><em>r<sub>i</sub></em></strong>— indices of socks which you should wear during the <strong><em>i</em></strong>-th day.




<strong>Output: </strong>

Print one integer — the minimum number of socks that should have their colours changed in order to be able to obey the instructions.




<strong>Example: Input: </strong>

4 3 3

1 2 3

<a href="#_Toc10922">1 2                                                                                                                                                                       1 </a>

<a href="#_Toc10923">1                                                                                                                                                                          2 </a>

<a href="#_Toc10924">2                                                                                                                                                                          3 </a>




3 1




<strong>Output: </strong>

1




<strong>Explanation:</strong> Put ‘2’ from second pair to the first pair. The first pair is then 2 2 and the second pair is 1 3 and the third pair is 3 1. Now, recolour sock ‘1’ to ‘3’ then your second pair is 3 3 and the third pair is also 3 3. You will be wearing the same colour of socks for two consecutive days. Thus, the situation is fixed by coloring only one sock.




<ol start="5">

 <li>Merging two arrays is an essential step in merge sort. Can we do the same in case of linked list? Given 2 sorted linked lists, devise a way to merge them while only using O(1) memory ?</li>

</ol>




<strong>Input: </strong>

First line contains the size of the first sorted array.

Second line contains the elements of the first sorted array.

Third line contains the size of the second sorted array.

Fourth line contains the elements of the second sorted array.




<strong>Output: </strong>

The final merged sorted array.




<strong>Example: </strong>

<strong>Input: </strong>

5

<ul>

 <li>2 3 4 5</li>

</ul>

6

<ul>

 <li>2 4 4 5 5</li>

</ul>




<strong>Output: </strong>

1 2 2 2 3 4 4 4 5 5 5




<ol start="6">

 <li>Sachin loved Gully Boy and he is now inspired to become a rapper. His friend Saurav gives him a string and asks him to rap it in his own way. Sachin, after some time, figures out that if there is a substring in that string which reads same even backwards sounds amazing. In order to impress the crowd, he decided to find the longest substring possible that contains half of the characters in proper alphabetical order. In other words, if the desired substring is of size <strong><em>2k</em></strong>, then the first <strong><em>k</em></strong> (<strong><em>k </em></strong>&gt; 1, i.e., the substring cannot be of size 2) characters are in proper alphabetical order. If there are two substrings possible with the same longest length, then print the one which comes first in alphabetical order. If no such substring can be found, print -1.</li>

</ol>

<strong>Input: </strong>

String s




<strong>Output: </strong>

The desired longest substring.




<strong>Example: Input: </strong>aaaabaaa




<strong>Output: </strong>aaabaaa




<strong>Input:</strong> abdccdba




<strong>Output:</strong>

-1 (Though the string is the same even when read backwards, but ‘d’ appears before ‘c’ in first half of the string. Note that ‘cc’ is not considered as the required substring.)




<strong>Input: </strong>

adsarttriopiuxyyxx




<strong>Output: </strong>rttr (Here, both rttr and xyyx read the same when read backwards. However, rttr precedes xyyx alphabetically.)







<ol start="7">

 <li>Sharat is currently at a car rental service, and he wants to reach a cinema hall. The film he has bought a ticket for starts in <strong><em>t</em></strong> minutes. There is a straight road of length <strong><em>s</em></strong> from the car rental service to the cinema. Let’s introduce a coordinate system so that the car rental service is at the point 0, and the cinema is at the point <strong><em>s</em></strong>. There are <strong><em>k</em></strong> gas stations along the road, and at each of them, you can fill a car with any amount of fuel for free! Consider that this operation doesn’t take any time, i.e. can be carried out instantly. There are <strong><em>n</em></strong> cars in the rental service, <strong><em>i</em></strong>-th of them is characterized with two integers <strong><em>c<sub>i</sub></em></strong> and <strong><em>v<sub>i</sub></em></strong> — the price of renting this car and the capacity of its fuel tank in litres. It is not possible to fuel a car with more fuel than its tank capacity <strong><em>v<sub>i</sub></em></strong>. All cars are have fuel filled to the full tank capacity at the car rental service. Each of the cars can be driven in one of two speed modes: normal or accelerated. In the normal mode, a car covers 1 kilometre in 2 minutes, and consumes 1 litre of fuel. In the accelerated mode, a car covers 1 kilometre in 1 minute, but consumes 2 litres of fuel. The driving mode can be changed at any moment and any number of times. Your task is to choose a car with minimum price such that Sharat can reach the cinema before the show starts, i.e. not later than in <strong><em>t</em></strong> minutes. Assume that all cars are completely fuelled initially.</li>

</ol>




<strong>Input: </strong>

The first line contains four positive integers <strong><em>n</em></strong>, <strong><em>k</em></strong>, <strong><em>s</em></strong> and <strong><em>t</em></strong> — the number of cars at the car rental service, the number of gas stations along the road, the length of the road and the time in which the film starts.

Each of the next <strong><em>n</em></strong> lines contains two positive integers <strong><em>c<sub>i</sub></em></strong> and <strong>v<sub>i</sub></strong>— the price of the <strong><em>i</em></strong>-th car and its fuel tank capacity.

The next line contains <strong><em>k</em></strong> distinct integers <strong><em>g<sub>1</sub></em></strong>, <strong><em>g<sub>2</sub></em></strong>, …, <strong><em>g<sub>k</sub></em></strong>— the positions of the gas stations on the road in arbitrary order.




<strong>Output: </strong>

Print the minimum rent price of an appropriate car, i.e. a car so that Sharat will be able to reach the cinema before the film starts (not later than <strong><em>t</em></strong> minutes). If there is no appropriate car, print -1.




<strong>Example: Input: </strong>

3 1 8 10

10 8

5 7

11 9

3




<strong>Output: </strong>

10




<ol start="8">

 <li>Captain America hasn’t given up the hope and is now looking for some ways to get back the infinity stones from Thanos. He goes to Titan to search for him but instead is stuck in a 2D string grid. After sending a distress signal to Captain Marvel, he receives a word. If that word exists in the grid, then Captain can come out otherwise not. The word can be constructed from horizontally or vertically neighbouring letters. Refer to sample cases for more clarity.</li>

</ol>




<strong>Note</strong> – The cell itself does not count as an adjacent cell. The same letter cell may be used more than once.




<strong>Input: </strong>

<strong><em>N</em></strong> (Number of strings) <strong><em>M</em></strong> (length of each strings)

Each of the next <strong><em>N</em></strong> lines would be strings with <strong><em>M</em></strong> length

<strong><em>T </em></strong>(Number of test cases)

Each of the next <strong><em>T</em></strong> lines would be words received from Captain marvel




<strong>Example:  </strong>

<strong>Input: </strong>

3 4

ABCE

SFCS

ADEE

5

ABCCED

SEE

ABCB

ABFSAB

ABCD




<strong>Output: </strong>

Yes

Yes

Yes

Yes

No




<ol start="9">

 <li>Imagine you have a special keyboard with the following keys:</li>

</ol>

Key 1:  Prints ‘A’ on screen

Key 2: (Ctrl-A): Select screen

Key 3: (Ctrl-C): Copy selection to buffer

Key 4: (Ctrl-V): Print buffer on screen appending it after what has already been printed.




Suppose you can only press the above mentioned four keys of the keyboard at most <strong><em>N</em></strong> times. Write a program to produce maximum numbers of A’s with <strong><em>N</em></strong> keystrokes. That is to say, the input parameter is <strong><em>N</em></strong> (no. of times you can press the keys), and the output is <strong><em>M</em></strong> (no. of A’s that you can produce).




<strong>Input: </strong>

The first line is <strong><em>N</em></strong> where N is the number of times key is pressed.




<strong>Output: </strong>

Print maximum number of As.  Print -1, if <strong><em>N</em></strong> is greater than 75.




<strong>Constraints: </strong>

1 ≤ <strong><em>N</em></strong> ≤ 75




<strong>Example: </strong>

<strong>Input: </strong>

3




<strong>Output: </strong>

3

<strong> </strong>

<strong>Explanation: </strong>Type 3 As by pressing Key 1 3 times.




<strong>Input: </strong>

7




<strong>Output: </strong>

9




<strong>Explanation: </strong>

Key 1 – print A, buffer – A

Key 2 – print A, buffer – AA

Key 3 – print A, buffer – AAA

Key 4 – select, buffer – AAA

Key 1 – copy, buffer – AAA

Key 1 – paste, buffer – AAAAAA

Key 1 – paste, buffer – AAAAAAAAA










****************************