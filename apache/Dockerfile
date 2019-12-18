FROM httpd:alpine

RUN sed -i '/LoadModule mpm_event_module/s/^#//g' /usr/local/apache2/conf/httpd.conf && \
    sed -i '/LoadModule rewrite_module/s/^#//g' /usr/local/apache2/conf/httpd.conf && \
    sed -i 's#AllowOverride [Nn]one#AllowOverride All#' /usr/local/apache2/conf/httpd.conf

#RUN echo "Include /usr/local/apache2/conf/redirect.conf" >> /usr/local/apache2/conf/httpd.conf
#COPY ./redirect.conf /usr/local/apache2/conf/redirect.conf
