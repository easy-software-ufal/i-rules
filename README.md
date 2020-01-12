## i-rules

### Improving Transformation Rules to Avoid Useless Mutants

\todo{Refazer o abstract apos finalizar o texto}
Mutation testing is a program-transformation technique that injects code changes to a program and checks whether these changes are caught by the existing test suite. 
Despite attracting a lot of interest because of its reputation as a powerful adequacy criterion for test suites, the costs of using mutation testing are usually high, hindering its use in industry. 
Useless mutants (eg., equivalents and duplicated) contribute to increase costs. 
An equivalent mutant is a mutant that has the same behavior of the original program. 
This way, this mutant is useless. A recent discovered kind of mutant is a mutant that has the same behavior of another one. 
They are duplicated and thus one of them is useless.

Previous research has focused mainly on detecting useless mutants only after they are generated and compiled. 

% In a previous work, we have introduced a strategy to help developers with deriving rules to avoid useless mutants right before their generation. We have discovered \NumberOfNewRules rules capable of avoiding useless mutants. All those rules were based on small, automatically-generated, Java programs. In this article, we extend the number of rules by discovering new ones based on manually-written Java programs.
In a previous work, we introduced a strategy to help developers with deriving rules to avoid useless mutants right before their generation. We discovered \NumberOfIdentifiedRules rules capable of avoiding useless mutants. All those rules were based on small, automatically-generated, Java programs. In this article, we augment our findings discovering new rules based on manually-written Java programs.
To use our strategy, we pass as input a set of programs. For each program, we also need a green test suite and a set of mutants. As output, our strategy yields a set of useless mutants candidates. After manually confirming that the mutants classified by our strategy as "useless" are indeed useless, we derive rules that can avoid their generation and thus decrease costs. 
In addition to the previously found rules, we increment new rules that can avoid useless mutants right before their generation. To evaluate if the rules found reduce the number of useless mutants generated, thus reducing the costs of the mutation testing, we enlarge the empirical evaluation implementing new rules (\todo{YY} more than our previous work) in the \mujava{} mutation testing tool.
We then take our \mujava{} version embedded with our rules and execute it in industrial-scale projects. Our rules reduced the number of mutants by almost \todo{XX}\% on average. 
While we cannot guarantee to generate only useful mutants, we can demonstrate a considerable reduction in the number of useless mutant generations, leading to substantial temporal savings.
Our results are promising because (i) we \textit{avoid} useless mutants generation; 
(ii) our strategy can help with identifying more rules in case we execute against a different set of Java programs; 
(iii) our \mujava{} version, embedded with the rules, takes less time to create and compile the mutants than the original version;
and (iv) we implement only a subset of the rules we derived. 

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Authors

Leo Fernandes - leonardo.oliveira@ifal.edu.br

Márcio Ribeiro - marcio@ic.ufal.br

Pedro Pinheiro - pmop@ic.ufal.br

Fabiano C. Ferrari - fcferrari@ufscar.br

Rohit Gheyi - rohit@dsc.ufcg.edu.br

André Santos - alms@cin.ufpe.br


Informatics Center, Federal University of Pernambuco---Recife, PE, Brazil

Informatics Coordination, Federal Institute of Alagoas---Macei\'o, AL, Brazil

Computing Institute, Federal University of Alagoas---Macei\'o, AL, Brazil

Computing Department, Federal University of S\~ao Carlos---S\~ao Carlos, SP, Brazil

Computing Departament, Federal University of Campina Grande---Campina Grande, PB, Brazil


### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
