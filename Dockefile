FROM uphold/litecoin-core:latest

ENV LITECOIN_DATA=/litecoin/.litecoin

RUN mkdir -p ${LITECOIN_DATA}

EXPOSE 9332 9333

ENTRYPOINT ["litecoind"]
CMD ["-server=1", "-txindex=1", "-rpcbind=0.0.0.0", "-rpcallowip=0.0.0.0/0", "-rpcuser=ltcuser", "-rpcpassword=ChangeThisToRandomPassword123!", "-printtoconsole"]
