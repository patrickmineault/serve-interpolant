# Serve interpolant

Rather than trying to implement interpolation on the client side, do it on the 
server side, where working with large(ish) files is not a problem. 

## Running the server locally

Drop the models (`interpolant_avg_diff.pkl` etc.) in models/

Install uvicorn in the local environment. Run:

```
uvicorn app:app --reload
```

Look at the docs at http://localhost:8000/docs

## Serving the API

Run `fly launch` the first time around, and `fly deploy` after that.