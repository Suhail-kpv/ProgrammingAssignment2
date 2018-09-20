CacheMatrix<-function(x=matrix()){
  invM<-NULL
  setM<-function(y){
    x<<-y
    invM<-NULL
  }
  getM<-function()x
    setInverse<-function(inverse)invM<<-inverse
    getInverse<-function()invM
    list(
      setM=setM,
      getM=getM,
      setInverse<-setInverse,
      getInverse<-getInverse,
      
    )
      
  
}
cacheSolve<-function(x,...){
  invM<-x$getInverse()
  if(!is.null(invM)){
    message("Getting Cached Data")
    return(invM)
  }
  mat<-x$get()
  invM<-solve(mat,...)
  x$getInverse(inv)
  inv
}
