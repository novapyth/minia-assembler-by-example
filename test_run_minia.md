
#1.test minia

/minia-v2.0.7-bin-Linux/bin/minia 

Specifiy -graph or -in

[minia options]


[assembly options]
          -graph            (1 arg) :    input graph file (hdf5)  [default '']
          -in               (1 arg) :    input reads (fasta/fastq/compressed)  [default '']
          -no-length-cutoff (0 arg) :    turn off length cutoff of 2*k in output sequences
          -traversal        (1 arg) :    traversal type ('contig', 'unitig')  [default 'contig']
          -starter          (1 arg) :    starting node ('best', 'simple')  [default 'best']
          -contig-max-len   (1 arg) :    maximum length for contigs  [default '0']
          -bfs-max-depth    (1 arg) :    maximum depth for BFS  [default '0']
          -bfs-max-breadth  (1 arg) :    maximum breadth for BFS  [default '0']
          -fasta-line       (1 arg) :    number of nucleotides per line in fasta output (0 means one line)  [default '0']

   [kmer count options]
          -kmer-size        (1 arg) :    size of a kmer  [default '31']
          -abundance-min    (1 arg) :    min abundance threshold for solid kmers  [default '3']
          -abundance-max    (1 arg) :    max abundance threshold for solid kmers  [default '4294967295']
          -histo-max        (1 arg) :    max number of values in kmers histogram  [default '10000']
          -solidity-kind    (1 arg) :    way to compute solids (sum, min or max)  [default 'sum']
          -max-memory       (1 arg) :    max memory (in MBytes)  [default '2000']
          -max-disk         (1 arg) :    max disk   (in MBytes)  [default '0']
          -solid-kmers-out  (1 arg) :    output file for solid kmers  [default '']
          -out              (1 arg) :    output file  [default '']
          -out-dir          (1 arg) :    output directory  [default '.']
          -minimizer-type   (1 arg) :    minimizer type (0=lexi, 1=freq)  [default '0']
          -minimizer-size   (1 arg) :    size of a minimizer  [default '8']
          -repartition-type (1 arg) :    minimizer repartition (0=unordered, 1=ordered)  [default '0']

   [bloom options]
          -bloom        (1 arg) :    bloom type ('basic', 'cache', 'neighbor')  [default 'neighbor']
          -debloom      (1 arg) :    debloom type ('none', 'original' or 'cascading')  [default 'cascading']
          -debloom-impl (1 arg) :    debloom impl ('basic', 'minimizer')  [default 'minimizer']

   [branching options]
          -branching-nodes (1 arg) :    branching type ('none' or 'stored')  [default 'stored']
          -topology-stats  (1 arg) :    topological information level (0 for none)  [default '0']

   [emphf options]
          -mphf (1 arg) :    mphf type ('none' or 'emphf')  [default 'emphf']

   [general options]
          -nb-cores          (1 arg) :    number of cores  [default '0']
          -verbose           (1 arg) :    verbosity level  [default '1']
          -integer-precision (1 arg) :    integers precision (0 for optimized value)  [default '0']

