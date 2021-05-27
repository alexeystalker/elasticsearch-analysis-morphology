# Morphological Analysis Plugin for ElasticSearch

The Morphological Analysis plugin integrates <a href="https://github.com/AKuznetsov/russianmorphology">Russian and English morphology for java and lucene framework</a> into elasticsearch. This plugin adds two new analyzers: "russian_morphology" and "english_morphology" and two token filters with the same names.

The <a href="https://github.com/DigDes/elasticsearch-analysis-morphology/blob/master/demo.sh">demo.sh</a> file shows a few examples of the analyzers behavior.


## Building
For building use latest gradle 6.6.1+ (https://gradle.org/install/#manually) and run
<pre>./gradlew build</pre>
Java SDK - tested on 15.

## Compatibility

Plugin is avaliable only for Elasticsearch 7.11.1.

Morphological Analysis Plugin | Elasticsearch   | URL  
--------| -------------|---------
7.6.0                            |7.6.0                |https://github.com/DigDes/elasticsearch-analysis-morphology/raw/master/analysis-morphology-7.6.0.zip
7.10.2                            |7.10.2              |https://github.com/DigDes/elasticsearch-analysis-morphology/raw/master/analysis-morphology-7.10.2.zip
7.11.1                           | 7.11.1   | https://github.com/sarafanfm/elasticsearch-analysis-morphology/raw/7.11.1/analysis-morphology-7.11.1.zip


## Installation

In order to install the plugin, simply run the following command in the elasticsearch home directory:
<pre>
bin/elasticsearch-plugin install file:///C:\PROJECTS\elasticsearch-analysis-morphology\analysis-morphology-7.11.1.zip
</pre>

where @zip_file_path@ is full path to zip archive with builded plugin.
Also, if you not know how build the plugin, the compiled version is added (analysis-morphology-7.11.1.zip)

P.S. I am not java developer, and I do not know about any errors. I am not tested yet the plugin, only install.