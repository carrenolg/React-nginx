################################## Stage 2 - deploy to production
FROM nginx:alpine

# remove default nginx configuration file
RUN rm /etc/nginx/conf.d/default.conf

# replace with custom one
COPY nginx.conf /etc/nginx/conf.d
