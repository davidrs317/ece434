FROM 
WORKDIR /usr/src/app

COPY . .

# RUN python -m venv venv
# RUN source venv/bin/activate
# RUN pip install --no-cache-dir -r packages.txt
# RUN pip install notebook
# RUN pip install pocketsphinx 

ENV VIRTUAL_ENV=/opt/venv
RUN python3 -m venv $VIRTUAL_ENV
ENV PATH="$VIRTUAL_ENV/bin:$PATH"
RUN pip install --no-cache-dir -r packages.txt

EXPOSE 8888

CMD ["jupyter", "notebook", "--allow-root" ]

