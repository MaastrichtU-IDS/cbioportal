FROM mysql:5.7.30

ADD https://github.com/cBioPortal/datahub/raw/master/seedDB/seed-cbioportal_hg19_v2.7.3.sql.gz /docker-entrypoint-initdb.d/
RUN chmod -R 777 /docker-entrypoint-initdb.d/seed-cbioportal_hg19_v2.7.3.sql.gz
ADD https://raw.githubusercontent.com/cBioPortal/cbioportal/v2.0.0/db-scripts/src/main/resources/cgds.sql /docker-entrypoint-initdb.d/
RUN chmod -R 777 /docker-entrypoint-initdb.d/cgds.sql