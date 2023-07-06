FROM busybox:latest
ENV NAMESPACE default
ENV CNLDAP admin
ENV DCLDAP dc=mycompany,dc=com
ENV LDAPPASSWD admin

RUN  mkdir /app /keys
WORKDIR /app
COPY main init.sh /app/
VOLUME /keys
EXPOSE 443
CMD ["./init.sh"] 

