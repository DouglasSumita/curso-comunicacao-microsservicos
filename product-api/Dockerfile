FROM gradle:7.3.3-jdk11
COPY --chown=gradle:gradle . .
WORKDIR .
RUN gradle build -x test --no-daemon
EXPOSE 8081
CMD [ "gradle", "bootRun" ]