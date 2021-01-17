FROM us.gcr.io/ib-trading-bot/cloud-run/base

# copy Python stuff and pip install packages
WORKDIR /home
COPY py .
RUN pip install -r requirements.txt

# execute cmd script to start Xvfb and gunicorn
CMD ./cmd.sh
