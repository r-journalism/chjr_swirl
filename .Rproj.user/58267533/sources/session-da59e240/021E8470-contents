keygen <- function(){
  set.seed(sum(as.numeric(charToRaw("Looking_at_Data"))))
  pran <- function(n = 1){
    replicate(n, sample(c(LETTERS, letters, 0:9), 1))
  }
  ks <- replicate(4, paste0(pran(4), collapse = ""))
  set.seed(NULL)
  pn <- sample(1:16, 1)
  kn <- sample(1:4, 1)
  sss <- paste(sample(c(LETTERS, letters, 0:9), 16-pn), collapse = "")
  eee <- paste(sample(c(LETTERS, letters, 0:9), pn), collapse = "")
  paste0(sss, ks[kn], eee)  
}

# Get the swirl state
getState <- function(){
  # Whenever swirl is running, its callback is at the top of its call stack.
  # Swirl's state, named e, is stored in the environment of the callback.
  environment(sys.function(1))$e
}

# Get the value which a user either entered directly or was computed
# by the command he or she entered.
getVal <- function(){
  getState()$val
}

# Get the last expression which the user entered at the R console.
getExpr <- function(){
  getState()$expr
}

get_coursera_log <- function(){
  clog_path <- file.path(getState()$udat, "rpe2.rds")
  if(!file.exists(clog_path)){
    clog <- data.frame(ln = c("Reading_Tabular_Data",
                              "Looking_at_Data",
                              "Data_Manipulation"), complete = rep("incorrect", 3),
                       stringsAsFactors = FALSE)
    saveRDS(clog, clog_path)
  }
  
  clog <- readRDS(clog_path)
  clog$complete[which(clog$ln == "Looking_at_Data")] <- "correct"
  saveRDS(clog, clog_path)
  clog
}
