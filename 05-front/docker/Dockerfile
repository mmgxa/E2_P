FROM public.ecr.aws/lambda/python:3.8

COPY ["requirements.txt", "./"]

RUN pip install --no-cache-dir -r requirements.txt

COPY ["lambda_function.py", "utils.py", "./"]

CMD [ "lambda_function.lambda_handler" ]