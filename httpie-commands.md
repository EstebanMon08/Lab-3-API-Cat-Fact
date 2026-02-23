export BASE_URL="https://catfact.ninja"
export RESOURCE="facts"

http GET $BASE_URL/$RESOURCE

http GET $BASE_URL/$RESOURCE limit==5

http GET $BASE_URL/$RESOURCE max_length==50 limit==3

http GET $BASE_URL/$RESOURCE page==2 limit==5

http GET $BASE_URL/breeds

http GET $BASE_URL/fakeendpoint

http GET $BASE_URL/$RESOURCE limit==abc

http GET $BASE_URL/$RESOURCE Authorization:"Bearer DEMO_TOKEN"

http GET $BASE_URL/$RESOURCE Authorization:"Bearer WRONGTOKEN"

http GET $BASE_URL/$RESOURCE max_length==100