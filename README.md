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
```sh
npm install npm@latest -g
```


<h2>Command line interface</h2>

<h2>References</h2>
