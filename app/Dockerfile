FROM rocker/shiny-verse:4.3.3
COPY . /srv/shiny-server/locret
WORKDIR /srv/shiny-server/locret
RUN R -e "install.packages(c('shiny', 'shinyWidgets', 'DT', 'plotly', 'bslib', 'shinyjs'), repos='https://cran.rstudio.com/')"
EXPOSE 3838
CMD ["/usr/bin/shiny-server"]
