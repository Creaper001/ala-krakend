FROM devopsfaith/krakend

COPY ./config ./etc/krakend/

ENV FC_ENABLE=1
ENV FC_OUT=/etc/krakend/krakend.json
ENV FC_PARTIALS=/etc/krakend/partials
ENV FC_SETTINGS=/etc/krakend/settings
ENV FC_TEMPLATES=/etc/krakend/templates

ENV KRAKEND_PORT=8080
ENV KRAKEND_DEBUG_ENDPOINT=false

EXPOSE 8080

CMD [ "run", "-d", "-c", "/etc/krakend/krakend.tmpl" ]
