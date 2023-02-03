<!-- HEARDERS -->
<div>
  <h1 align="center">G2P Model<br />
  From Genome to Pixels Model</h1>

  <p align="center">
    <b>An approach to transform Genomes into 2-Dimensional Images</b>
    <br />
    <br />
    <img height="500px" src='images/G2P_2.png' />
  </p>
</div>


<!-- CONTENT -->
<h1 >Getting Started</h1>
The G2P tool allows to extract images from any fasta files, containing set of nucleotides (A, T, C ang G).
The model can exploit well-known indicators in the field, to create contrast and bring out the breaking points in the final image, and consequently in the genome.
<br />
The tool relies on three parameters:
<ul>
  <li><b>The genome (GN):</b><br />
    that correspond to the .fasta file containing the whole genome as a sequence of nucleobases (A, T, C ang G).
  </li>
  
  <li><b>The portion size (S):</b><br />
     the given size used to extract portions of the genome, used to encode each pixel.
  </li>
  
  <li><b>Transformation function (T):</b><br />
     that transforms each genome sub-sequence of size S it into an integer representing the color of a pixel.
  </li>
</ul>

By this way, the G2P Tool allows to extract several representations of a same genome according to the feature that want to be highlighted.

The application can be used in Graphical modes and in commande line interface (CLI).


<h2>Graphic interface</h2>
The graphical mode can be started by double-clicking on the file <b><i>G2P-Model.jar</i></b> or by using the commande
<br />
<br />
  
```sh
java -jar G2P-Model.jar
```

Note that in both case the directory <b><i>images</i></b> must be in the same directory than the <b><i>G2P-Model.jar</i></b> file.

Once the interface is started, a fasta file containing the genome must be loaded to begin. 
It can be loaded by using the <b><i>Menu</i></b> or the <b><i>Tool bar</i></b>.




<h2>Command line interface</h2>

In commande line, the tool can be used as follow 

```sh
java -jar G2P-Model.jar <genome> <transformationFunction> <portionSize> <resultingImage>
```

<ul>
  <li><b>genome:</b><br />
    that correspond to the <b><i>.fasta file</b></i> containing the whole genome as a sequence of nucleobases (A, T, C ang G).
  </li>
  
  <li><b>transformationFunction:</b><br />
     the transformation function used (between: sum, chaffgard, skew, component, diversity, distance, nuclescore)
  </li>
  
  <li><b>portionSize:</b><br />
     the size of the subsequence used to encode each pixel (between: 1 and 100 000).
  </li>

  <li><b>resultingImage:</b><br />
     name of the resulting image file.
  </li>
</ul>

Note that the resulting image is created, as a <b><i>.png</b></i> file, in the same reporty than the genome file.


<h2>Transformation function implemented</h2>
In the current version of the application, several transformation functions have been implemented



<h2>References</h2>

<ol>
  <li>Thomas A Clarke and Laurence D Hurst. Gc-content evolution in prokaryotes and eukaryotes: a tale of two genomes. Trends in genetics, 22(11):632–640, 2006
  </li>
  
  <li> Kazuharu Arakawa and Masaru Tomita. The gc skew index: a measure of genomic compositional asymmetry and the degree of replicational selection. Evolutionary Bioinformatics, 3:117693430700300006, 2007
  </li>
  
  <li> Jan Mrazek and Samuel Karlin. Strand compositional asymmetry in bacterial and large viral genomes. Proceedings of the National Academy of Sciences, 95(7):3720–3725, 1998
  </li>
  
  <li>
    José Manuel Peregr ́ın-  ́Alvarez and John Parkinson. The global landscape of sequence diversity. Genome biology, 8(11):1–17, 2007
   </li>
</ol>
