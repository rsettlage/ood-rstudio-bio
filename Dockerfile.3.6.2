## helpful read: https://divingintogeneticsandgenomics.rbind.io/post/run-rstudio-server-with-singularity-on-hpc/
## combining the tidyverse and verse Dockerfiles, wanting to make sure I have the rstudio-r version

FROM rsettlag/ood-rstudio-basic:3.6.2

LABEL org.label-schema.license="GPL-2.0" \
      org.label-schema.vcs-url="https://github.com/rsettlag" \
      maintainer="Robert Settlage <rsettlag@vt.edu>"

RUN apt-get update -qq && apt-get -y --no-install-recommends install \
  libxml2-dev \
  libcairo2-dev \
  libsqlite3-dev \
  libmariadbd-dev \
##  libmariadb-client-lgpl-dev \
  ## replaced by  this one maybe
  libmariadb-client-lgpl-dev-compat \
  libpq-dev \
  libssh2-1-dev \
  mesa-common-dev \
  libglu1-mesa-dev \
  unixodbc-dev \
  libsasl2-dev \
  libhdf5-dev \
  curl \
  rustc \
  bzip2 \
  php \
  php-common \
  imagemagick \
  php-imagick
 
RUN echo "options(repos = c(CRAN='https://cran.rstudio.com'), download.file.method = 'libcurl')" >> /usr/local/lib/R/etc/Rprofile.site

RUN Rscript -e "BiocManager::install(update=TRUE,ask=FALSE,lib.loc='/usr/local/lib/R/site-library/',c('kableExtra','tidyverse','dplyr','devtools','formatR','remotes','selectr','caTools','ggpubr','data.table','lme4','VennDiagram','doParallel','gplots','ape','metap','bigmemory','circlize','dendextend','flashClust','ggrepel','randomForest','parallelDist','pvclust','Rtsne','vegan','zoo','igraph','rlecuyer','tibble','car','RcppEigen','crosstalk','sctransform','uwot','GenomicAlignments','Rsamtools','multtest','rtracklayer','seqinr','micropan','phangorn','phytools','Biostrings','Biobase','MLSeq','biomaRt','DESeq2','DT','edgeR','goseq','gplots','gtools','Heatplus','rwantshue','WGCNA','Seurat'))" 

RUN Rscript -e "devtools::install_github('hoesler/rwantshue')"

RUN apt-get clean \
  && rm /usr/local/lib/R/etc/Rprofile.site


