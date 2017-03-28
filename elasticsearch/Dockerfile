FROM elasticsearch:5

ENV ES_JAVA_OPTS="-Des.path.conf=/etc/elasticsearch"
elasticsearch-plugin install analysis-icu
elasticsearch-plugin install X-Pack 
elasticsearch-plugin install Kuromoji
elasticsearch-plugin install mobz/elasticsearch-head
CMD ["-E", "network.host=0.0.0.0", "-E", "discovery.zen.minimum_master_nodes=1"]
