

# receive file

# extract content

# split content -> chunks -> 1000 char each

# convert each chunk to vector

# store vecors in db
createunique id for file
file_id = uuid.uuid4()

for chunk in chunks:

    test_cllection.add( 
                        ids=[ str(id) ], 
                        documents=[chunk], 
                        embeddings=[vectors.data[0].embedding], 
                        metadata=[ { "document_id":  "doc_123"  } ] 
                    )

# delete or update


collction_name.delete( where={"document_id":  "doc_123"} )

# 


